<template>
  <div id="navbar-wrapper">
    <ul id="navbar" dir="rtl">
			<li class="navbar-item"><a href="">ראשי</a></li>
			<li class="navbar-item" id="detail-item">
				<a href="">התמחות המשרד <i class="fas fa-chevron-down"></i></a>
				<ul id="more">
					<li id="more-crime">
						<p class="category-title">משפט פלילי</p>
						<ul id="more-crime-lists">
							<li class="arrests-list">
								<p class="subcategory">חקירות ומעצרים</p>
								<ArrestsList/>
							</li>
							<li class="criminal-list">
								<p class="subcategory">עבירות פליליות</p>
								<CriminalList/>
							</li>
							<li class="other-list">
								<p class="subcategory">תחומי עיסוק נוספים</p>
								<OtherList/>
								<a href="#" class="show-more">לרשימה מלאה <i class="fas fa-arrow-left"></i></a>
							</li>
						</ul>
					</li>
					<li class="military-list">
						<p class="category-title">משפט צבאי</p>
						<MilitaryList/>
					</li>
					<li class="traffic-list">
						<p class="category-title">משפט תעבורה</p>
						<TrafficList/>
					</li>
				</ul>
			</li>

			<li class="navbar-item"><a href="">אודות</a></li>
			<li class="navbar-item"><a href="">פרסומים</a></li>
			<li class="navbar-item"><a href="">בלוג</a></li>
			<li class="navbar-item"><a href="">פורום</a></li>
			<li class="navbar-item"><a href="">הצלחות</a></li>
			<li class="navbar-item"><a href="">המלצות</a></li>
			<li class="navbar-item"><a href="">צור קשר</a></li>
			<li class="navbar-item pop-up-button"><button @click="popup = !popup">ייעוץ ראשוני <i class="fas fa-chevron-left"></i></button></li>
		</ul>
		<div id="popup-wrapper" v-if="popup">
      <div id="popup">
        <img src="img/‏‏‏‏‏‏‏‏home/01/pop_up.png" alt="pop_up">
        <form action="submit" dir="rtl" id="popup-form">
          <h4>לייעוץ ראשוני השאירו פרטים</h4>
					<input type="text" placeholder="שם מלא *">
					<input type="text" placeholder="נייד *">
					<select name="time select">
						<option value="placeholder" selected>בחר שעה לחזרה</option> 
						<option value="morning">Morning</option>
						<option value="day">Day</option>
						<option value="evening">Evening</option>
					</select>
					<button>תחזרו אליי <i class="fas fa-chevron-left"></i></button>
				</form>
        <button id="close-btn" @click="popup = !popup"><i class="fas fa-times"></i></button>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
@import '@/variables.scss';
#navbar-wrapper {
	border-top: 1px solid #e1e1e1;
	height: 55px;
}

#navbar {
	@include flex;
	height: 100%;
	font-size: 15px;
	margin: 0;
	padding: 0;
	list-style-type: none;
}

.navbar-item {
	height: 100%;
	padding: 0 2%;
	
	&:hover {
		background: #ebeef1;
	}

	a {
		color: $main-color;
		font-size: 19px;
		line-height: 55px;

		i {
			font-size: 10px;
		}
	}
}

.pop-up-button {
	background: $main-color;

	button {
		background: transparent;
		border: none;
		font-family: $font-bold;
		color: $light-color;
		font-size: 19px;
		line-height: 55px;
		outline: none;
	}

	&:hover {
		background: $main-color;
	}
}

.category-title {
	color: $light-color;
	font-size: 22px;
	text-align: center;
	line-height: 50px;
	border-bottom: 1px solid rgba(76, 86, 100, 0.53);
}

.subcategory {
	color: $light-color;
	font-size: 18px;
}

#detail-item:hover #more {
	@include flex(row, space-between, flex-start);
	position: absolute;
	z-index: 1;
}

#more {
	display: none;
	list-style-type: none;
	position: absolute;
	left: 0;
	right: 0;

	a {
		opacity: 0.5;
		color:$light-color;
		font-size: 15px;
		line-height: 25px;

		&:hover {
			opacity: 1;
		}
	}

	&-crime {
		@include flex(column, flex-start, stretch);
		padding-bottom: 0;
		height: 100%;
		background: #061a2d;
		width: 66%;


		&:hover &-lists {
			@include flex(row, space-between, flex-start);
		}

		&-lists {
			display: none;
			list-style-type: none;
			height: 100%;

			.criminal-list {
				width: 50%;
				padding-top: 25px;
			}

			.arrests-list, .other-list {
				width: 25%;
				padding: 25px 25px 0 0;
				@include flex(column, flex-start, stretch)
			}

			.show-more {
				opacity: 1;

				i {
					font-size: 8px;
				}
			}

			.criminal-list, .other-list {
				border-right: 1px solid rgba(76, 86, 100, 0.53);
				padding-right: 25px;
				box-sizing: border-box;
				height: 100%;
			}
		}
	}

	.military-list, .traffic-list {
		width: 17%;
			background: #061a2d;
		
		ul {
			display: none;
			padding-bottom: 15px;
		}

		&:hover ul {
			display: block;
		} 
	} 

}

#popup-wrapper {
    @include flex(row, center, center);
    position: fixed;
    left: 0;
    top: 0;
    z-index: 10;
    width: 100vw;
    height: 100vh;
    background: rgba(0, 0, 0, 0.6);

    #popup {
      width: 732px;
      height: 365px;
      position: relative;
      @include flex;

      img {
        width: 50%;
        height: 100%;
      }
    }

    #popup-form {
      width: 50%;
      height: 100%;
      @include flex(column, center);
      background: white;

      input {
        width: 255px;
        height: 44px;
        background-color: #f3f6f8;
        color: #454545;
        font-family: $font;
        font-size: 17px;
        border: none;
        padding-right: 15px;
        margin: 10px;

        &::placeholder {
          color: #454545
        }
      }

      select {
        width: 270px;
        height: 44px;
        background-color: #f3f6f8;
        border: none;
        color: #454545;
        font-size: 17px;
        margin: 10px;
      }

      button {
        width: 147px;
        height: 44px;
        background-color: #007eef;
        border: none;
        padding: 0;
        color: #ffffff;
        font-family: $font-bold;
        font-size: 19px;

        i {
          font-size: 9px;
        }
      }

      h4 {
        color: $main-color;
        font-family: $font-bold;
        font-size: 24px;
        font-weight: 400;
        line-height: 45px;
        margin: 0;
      }
    }

    #close-btn {
      background: transparent;
      font-size: 19px;
      color: rgba(255, 255, 255, 0.6);
      outline: none;
      border: none;
      position: absolute;
      right: -22px;
      top: -22px;

    }
  }


	@media screen and (max-width: 500px) {
		#navbar-wrapper {
			display: none;
		}
	}
</style>

<script>

import ArrestsList from '@/components/header/Navbar/ArrestsList'
import CriminalList from '@/components/header/Navbar/CriminalList'
import MilitaryList from '@/components/header/Navbar/MilitaryList'
import OtherList from '@/components/header/Navbar/OtherList'
import TrafficList from '@/components/header/Navbar/TrafficList'

export default {
	name: 'navbar',
	data: () => ({
		popup: false
	}),
  components: {
   ArrestsList, CriminalList, MilitaryList, OtherList, TrafficList
  }
}
</script>