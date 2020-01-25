<template>
  <div class="navbar-wrapper-mobile">
    <ul class="navbar-mobile" dir="rtl">
      <li class="navbar-item-mobile" v-if="menu1"><a href="" class="category-name-mobile">ראשי</a></li>


      <li class="detail-item-mobile" :class="{ open_menu: menu3 || menu4 || menu5 }">
        <button class="category-name-mobile detail-btn-mobile" @click="OpenMenu2">
					<i class="fas fa-arrow-right" v-if="menu2"></i>
					התמחות המשרד 
					<i class="fas fa-chevron-left" v-if="menu1"></i>
				</button>
        <ul class="more-mobile" v-if="menu2">
          <li class="more-crime-mobile navbar-item-mobile" :class="{ open_submenu: menu3 }">
						<button class="navbar-item-mobile category-name-mobile category-title-mobile" @click="OpenMenu3">
							משפט פלילי
							<i class="fas fa-chevron-down" v-if="!menu3"></i>
							<i class="fas fa-chevron-up" v-if="menu3"></i>
							</button>
            <ul class="more-crime-lists-mobile" :class="{ lower_open_menu: menu3 }" v-if="menu3">
              <li class="arrests-list-mobile">
                <p class="subcategory-mobile">חקירות ומעצרים</p>
                <ArrestsList/>
              </li>
              <li class="criminal-list-mobile" v-if="menu2">
                <p class="subcategory-mobile">עבירות פליליות</p>
                <CriminalList/>
              </li>
              <li class="other-list-mobile" v-if="menu2">
                <p class="subcategory-mobile">תחומי עיסוק נוספים</p>
                <OtherList/>
                <a href="#" class="show-more-mobile">לרשימה מלאה <i class="fas fa-arrow-left"></i></a>
              </li>
            </ul>
          </li>
          <li class="military-list-mobile navbar-item-mobile" :class="{ open_submenu: menu4 }">
						<button class="navbar-item-mobile category-name-mobile category-title-mobile" @click="OpenMenu4">
							משפט צבאי
							<i class="fas fa-chevron-down" v-if="!menu4"></i>
							<i class="fas fa-chevron-up" v-if="menu4"></i>
						</button>
            <MilitaryList class="military-list-component-mobile" v-if="menu4"></MilitaryList>
          </li>
          <li class="traffic-list-mobile navbar-item-mobile" :class="{ open_submenu: menu5 }">
						<button class="navbar-item-mobile category-name-mobile category-title-mobile" @click="OpenMenu5">
							משפט תעבורה
							<i class="fas fa-chevron-down" v-if="!menu5"></i>
							<i class="fas fa-chevron-up" v-if="menu5"></i>
						</button>
            <TrafficList class="traffic-list-component-mobile" v-if="menu5"></TrafficList>
          </li>
        </ul>
      </li>

      <li class="navbar-item-mobile" v-if="menu1"><a href="" class="category-name-mobile">אודות</a></li>
      <li class="navbar-item-mobile" v-if="menu1"><a href="" class="category-name-mobile">פרסומים</a></li>
      <li class="navbar-item-mobile" v-if="menu1"><a href="" class="category-name-mobile">בלוג</a></li>
      <li class="navbar-item-mobile" v-if="menu1"><a href="" class="category-name-mobile">פורום</a></li>
      <li class="navbar-item-mobile" v-if="menu1"><a href="" class="category-name-mobile">הצלחות</a></li>
      <li class="navbar-item-mobile" v-if="menu1"><a href="" class="category-name-mobile">המלצות</a></li>
      <li class="navbar-item-mobile" v-if="menu1"><a href="" class="category-name-mobile">צור קשר</a></li>
      <select name="lang" dir="ltr" class="select-mobile" v-if="menu1">
        <option value="HE" selected>HE</option> 
        <option value="EN">EN</option>
        <option value="FR">FR</option>
        <option value="RU">RU</option>
      </select>
    </ul>
  </div>
</template>

<script>

import ArrestsList from '@/components/header/Navbar/ArrestsList'
import CriminalList from '@/components/header/Navbar/CriminalList'
import MilitaryList from '@/components/header/Navbar/MilitaryList'
import OtherList from '@/components/header/Navbar/OtherList'
import TrafficList from '@/components/header/Navbar/TrafficList'

export default {
  name: 'navbarMob',
  data: () => ({
		menu1: true,
		menu2: false,
		menu3: false,
		menu4: false,
		menu5: false
	}),
	methods: {
		OpenMenu2 () {
			this.menu2 = !this.menu2,
			this.menu1 = !this.menu1,
			this.menu3 = false,
			this.menu4 = false,
			this.menu5 = false
		},
		OpenMenu3 () {
			if (this.menu3 === false) {
				this.menu3 = true,
				this.menu4 = false,
				this.menu2 = true,
				this.menu5 = false
			} else {
				this.menu3 = !this.menu3,
				this.menu2 = true
			}
		},

		OpenMenu4 () {
			if (this.menu4 === false) {
				this.menu4 = true,
				this.menu3 = false,
				this.menu2 = true,
				this.menu5 = false
			} else {
				this.menu4 = !this.menu4,
				this.menu2 = true
			}
		},
		OpenMenu5 () {
			if (this.menu5 === false) {
				this.menu5 = true,
				this.menu4 = false,
				this.menu2 = true,
				this.menu3 = false
			} else {
				this.menu5 = !this.menu5,
				this.menu2 = true
			}
		}	
  },
  components: {
   ArrestsList, CriminalList, MilitaryList, OtherList, TrafficList
  }
}

</script>

<style lang="scss">
@import '@/variables.scss';

.navbar-wrapper-mobile {
  width: 258px;
  height: 100vh;
  position: fixed;
  z-index: 11;
  top: 0;
  right: 0;
  background-color: #061a2d;
}

.navbar-mobile {
  @include flex(column, flex-start, flex-start);
  height: 100%;
  width: 100%;
}

.navbar-item-mobile, .category-title-mobile {
  height: 57px;
  width: 100%;
  padding: 0;
  border-bottom: 1px solid rgba(133, 132, 132, 0.2);
}

.category-name-mobile {
  font-size: 19px;
  line-height: 27px;
  color: $light-color;
  width: 100%;
  height: 55px;
  @include flex;
  padding: 0 20px;
  box-sizing: border-box;
	border: none;
	background: transparent;
}

.subcategory-mobile {
  color: $light-color;
  font-size: 16px;
	margin-top: 30px;
}

.detail-item-mobile {
  width: 100%;
  padding: 0;

	.detail-btn-mobile {
		border-bottom: 1px solid rgba(133, 132, 132, 0.2);
	}
}
.more-mobile {

	.more-crime-lists-mobile {
		height: 430px;
		overflow: auto;
	}
		
  a {
    opacity: 0.5;
    color:$light-color;
    font-size: 15px;
    line-height: 25px;

    &:hover {
      opacity: 1;
    }
  }
}
	
.military-list-mobile ul, .traffic-list-mobile ul, .criminal-list-mobile, .other-list-mobile, .arrests-list-mobile {
	padding: 0 20px;
}

.select-mobile {
  width: 50px;
  color: white;
  font-size: 19px;
  border: none;
  outline: none;
	background-color: #061a2d;
	position: absolute;
	bottom: 41px;
	right: 25px;

	option {
		background-color: #061a2d;
	}
}
.open_menu {
	height: 100%;
}
.open_submenu {
	height: 490px;
}
.lower_open_menu {
	height: 430px;
}
</style>