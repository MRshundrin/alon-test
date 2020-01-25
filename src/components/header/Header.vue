<template>
  <header id="header-wrapper">
    <div id="header-main">
      <div id="header-main-top">
        <div id="phone-number">
          <span id="number">050-7368203</span>
          <i class="fas fa-phone"></i>
          זמין <span id="selected-text">24 שעות</span> ביממה
        </div>
        <div id="lang-search">
          <select name="lang" id="lang">
            <option value="HE" selected>HE</option> 
            <option value="EN">EN</option>
            <option value="FR">FR</option>
            <option value="RU">RU</option>
          </select>
        
          <form id="search-form">
            <input type="text" placeholder="חיפוש באתר" dir="rtl">
            <button class="search-button"></button>
          </form>
        </div>
      </div>
      <NavbarMobile v-if="mobile && mobileMenu"></NavbarMobile>
      <Navbar v-if="desktop"></Navbar>
      <button id="mobile-btn-menu" @click="menu"><img src="img/‏‏‏‏‏‏‏‏home/01/mobile_button_menu.png" alt="logo"></button>
      <button id="close-menu-btn" @click="menu" v-if="mobile && mobileMenu"><i class="fas fa-times"></i></button>
    </div>
    <img src="img/‏‏‏‏‏‏‏‏home/01/logo.png" alt="logo" id="header-logo">
  </header>
</template>

<style lang="scss">
@import '@/variables.scss';

#header-wrapper {
  width: 72%;
  margin: 0 auto;
  @include flex;

  #header-main {
    width: 81%;
    border-right: 1px solid #e1e1e1;
    align-self: stretch;
    @include flex (column, center, stretch);

    &-top {
      width: 100%;
      height: 54px;
      @include flex;
      
      #phone-number {
        flex-shrink: 0;
        color: $main-color;
        margin-right: 21px;
        font-family: $font-bold;
        font-size: 20px;
        line-height: 30px;

        i {
          font-size: 16px;
        }

        #selected-text {
          color: #007eef;
        }

        #number {
          font-size: 27px;
        }
      }

      #lang-search {
        width: 70%;
        align-self: stretch;
        @include flex;

        select {
          width: 72px;
          color: $main-color;
          font-size: 19px;
          border: none;
          border-left: 1px solid #e1e1e1;
          align-self: stretch;
          outline: none;

          option {
            background: #ebeef1;
          }
        }

        #search-form {
          margin-right: 31px;
          input {
            height: 18px;
            opacity: 0.54;
            color: #00284c;
            font-family: $font;
            margin-right: 13px;
            font-size: 19px;
            border: none;
            outline: none;

          }
          button {
            width: 18px;
            height: 18px;
            border: none;
            background: none;
            outline: none;

            background-image: url(../../../public/img/‏‏‏‏‏‏‏‏home/01/search.png);

            &:active {
              background-image: url(../../../public/img/‏‏‏‏‏‏‏‏home/01/search_active.png);
            }
          }

        }
      }
    }

    #mobile-btn-menu {
      display: none;
    }

    &-bottom {
      height: 54px;
    }
  }
}

#close-menu-btn {
  display: none;
}

// mobile version

@media screen and (max-width: 500px) {
  #header-wrapper {
    width: 100%;
    box-sizing: border-box;
    @include flex(row-reverse);

    #header-logo {
      width: 133px;
      height: 44px;
      margin-left: 5px;
    }

    #header-main {
      width: 75px;
      border: 0;

      #header-main-top {
        display: none;
      }

      #mobile-btn-menu {
        display: block;
        width: 70px;
        height: 65px;
        border: none;
        outline: none;
        background: transparent;
        padding: 0;
        border-left: 2px solid #e1e1e1;
      }
    }
  }

  #close-menu-btn {
    display: block;
    width: 65px;
    height: 65px;
    position: fixed;
    top: 0;
    right: 257px;
    z-index: 5;
    background: white;
    font-size: 24px;
    border: none;
  }
}
</style>

<script>


import NavbarMobile from '@/components/header/Navbar/NavbarMobile'
import Navbar from '@/components/header/Navbar/Navbar'

export default {
  name: 'headerMain',
  data: () => ({
    openMobile: false,
    mobile: false,
    mobileMenu: false,
    desktop: true,
    windowWidth: window.innerWidth
  }),
  methods: {
    menu () {
      if (this.mobile) {
        this.mobileMenu = !this.mobileMenu
      }
    }
  },
  mounted () {
    window.onresize = () => {
      this.windowWidth = window.innerWidth;
      if (this.windowWidth > 500) {
        this.desktop = true;
        this.mobile = false;
      } else {
        this.desktop = false;
        this.mobile = true;
      }
    };
  },
  
  components: {
   Navbar, NavbarMobile
  }
}
</script>