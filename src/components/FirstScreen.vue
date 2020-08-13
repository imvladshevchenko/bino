<template>
  <div class="first-screen">
    <div class="container">
      <div class="hamburger-menu" id="burger">
        <a class="hamburger-menu__title" href="#">
          <img src="../img/header/logo.png" alt="logo" />
        </a>
        <input id="menu__toggle" type="checkbox" />
        <label class="menu__btn" for="menu__toggle">
          <span></span>
        </label>
        <ul class="menu__box">
          <li><a class="menu__item" href="#">Home</a></li>
          <li><a class="menu__item" href="#products">ABOUT US</a></li>
          <li><a class="menu__item" href="#FAQ">PORTFOLIO</a></li>
          <li><a class="menu__item" href="#footer">PRICING</a></li>
          <li><a class="menu__item" href="#">BLOG</a></li>
          <li><a class="menu__item" href="#">CONTACT</a></li>
        </ul>
      </div>
      <div class="first-screen__navigation" id="navBar">
        <a href="" class="first-screen__logo-wrapper">
          <img src="../img/header/logo.png" alt="logo" />
        </a>
        <ul class="first-screen__list">
          <li class="first-screen__list-item">
            <a href="" title="HOME" class="first-screen__nav">HOME</a>
          </li>
          <li class="first-screen__list-item">
            <a href="" title="ABOUT US" class="first-screen__nav">ABOUT US</a>
          </li>
          <li class="first-screen__list-item">
            <a href="" title="PORTFOLIO" class="first-screen__nav">PORTFOLIO</a>
          </li>
          <li class="first-screen__list-item">
            <a href="" title="PRICING" class="first-screen__nav">PRICING</a>
          </li>
          <!-- <li class="first-screen__list-item">
            <a href="" title="TEAM" class="first-screen__nav">TEAM</a>
          </li> -->
          <li class="first-screen__list-item">
            <a href="" title="BLOG" class="first-screen__nav">BLOG</a>
          </li>
          <li class="first-screen__list-item">
            <a href="" title="CONTACT" class="first-screen__nav">CONTACT</a>
          </li>
        </ul>
      </div>
      <div uk-slider class="slider-container">
        <ul class="uk-slider-items slider">
          <li class="slider__item item1">
            <div class="first-screen__title-wrapper">
              <h4 class="first-screen__subtitle">
                Our Clients Are Our First Priority
              </h4>
              <h1 class="first-screen__title">WELCOME TO BINO</h1>
              <div class="first-screen__dot"></div>
              <p class="first-screen__text">
                Lorem Ipsum is simply dummy text of the printing and typesetting
                industry. Lorem Ipsum has been the industry's standard dummy
                text ever since the 1500s, when an unknown printer took a galley
                of type and scrambled it to make a type specimen book.
              </p>
              <div class="first-screen__links-wrapper">
                <a href="" class="button first-screen__button"
                  >GET STARTED NOW</a
                >
                <a href="" class="button first-screen__button">LEARN MORE</a>
              </div>
            </div>
          </li>
          <li class="slider__item item2">
            <div class="first-screen__title-wrapper">
              <h4 class="first-screen__subtitle">
                Our Clients Are Our First Priority
              </h4>
              <h1 class="first-screen__title">WELCOME TO BINO</h1>
              <div class="first-screen__dot"></div>
              <p class="first-screen__text">
                Lorem Ipsum is simply dummy text of the printing and typesetting
                industry. Lorem Ipsum has been the industry's standard dummy
                text ever since the 1500s, when an unknown printer took a galley
                of type and scrambled it to make a type specimen book.
              </p>
              <div class="first-screen__links-wrapper">
                <a href="" class="button first-screen__button"
                  >GET STARTED NOW</a
                >
                <a href="" class="button first-screen__button">LEARN MORE</a>
              </div>
            </div>
          </li>
          <li class="slider__item item3">
            <div class="first-screen__title-wrapper">
              <h4 class="first-screen__subtitle">
                Our Clients Are Our First Priority
              </h4>
              <h1 class="first-screen__title">WELCOME TO BINO</h1>
              <div class="first-screen__dot"></div>
              <p class="first-screen__text">
                Lorem Ipsum is simply dummy text of the printing and typesetting
                industry. Lorem Ipsum has been the industry's standard dummy
                text ever since the 1500s, when an unknown printer took a galley
                of type and scrambled it to make a type specimen book.
              </p>
              <div class="first-screen__links-wrapper">
                <a href="" class="button first-screen__button"
                  >GET STARTED NOW</a
                >
                <a href="" class="button first-screen__button">LEARN MORE</a>
              </div>
            </div>
          </li>
        </ul>
        <a
          class="uk-position-center-left uk-position-small slidenav slidenav-previous"
          href=""
          uk-slidenav-previous
          uk-slider-item="previous"
          ><i class="fas fa-angle-left"></i
        ></a>
        <a
          class="uk-position-center-right uk-position-small slidenav slidenav-next"
          href=""
          uk-slidenav-next
          uk-slider-item="next"
          ><i class="fas fa-angle-right"></i
        ></a>
      </div>
    </div>
    <a href="#what-we-do" class="first-screen__scroll-down">
      <img src="../img/header/Forma1.png" alt="scroll" />
    </a>
  </div>
</template>

<script>
export default {
  name: "FirstScreen",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container {
  width: 100%;
  height: 100vh;
  padding-top: 40px;
}
$styles: first-screen;
.#{$styles} {
  &__navigation {
    display: none;
    @media screen and (min-width: 1023px) {
      padding: 0 15px;
      width: 100%;
      max-width: 1170px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      z-index: 10;
      position: absolute;
      left: 50%;
      transform: translateX(-50%);
    }
  }
  &__list {
    display: flex;
    flex-direction: row;
    list-style: none;
  }
  &__list-item:not(:last-child) {
    margin-right: 55px;
  }
  &__nav {
    position: relative;
    text-decoration: none;
    font-family: $base-font;
    font-size: $H14;
    color: $NL1;
    &::before {
      content: "";
      display: inline-block;
      position: absolute;
      left: 0;
      right: 0;
      top: 46px;
      height: 1px;
      background-color: transparent;
      transition: all 0.2s ease;
    }
    &::after {
      display: block;
      content: attr(title);
      font-weight: bold;
      height: 0;
      overflow: hidden;
      visibility: hidden;
    }
    &:hover {
      text-shadow: 0;
      font-weight: bold;
      &:before {
        color: $R1;
        background-color: $R1;
      }
    }
  }
  &__title-wrapper {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  &__subtitle {
    font-family: $sec-font;
    font-size: $H24;
    letter-spacing: 1.2px;
    color: $NL1;
    margin-bottom: $H45;
  }
  &__title {
    font-family: $base-font;
    font-size: $H45;
    letter-spacing: 7.2px;
    color: $NL1;
    margin-bottom: $H45;
    text-transform: uppercase;
    font-weight: bold;
    @media screen and (min-width: 992px) {
      font-size: $H72;
    }
  }
  &__dot {
    position: relative;
    display: flex;
    border-radius: 50%;
    width: $H8;
    height: $H8;
    background-color: $R1;
    margin-bottom: $H45;
    &::after {
      content: "";
      display: block;
      position: absolute;
      width: 80px;
      height: 2px;
      background-color: $NL3;
      top: 50%;
      transform: translateY(-50%);
      left: 22px;
    }
    &::before {
      content: "";
      display: block;
      position: absolute;
      width: 80px;
      height: 2px;
      background-color: $NL3;
      top: 50%;
      transform: translateY(-50%);
      right: 22px;
    }
  }
  &__text {
    max-width: 584px;
    font-family: $base-font;
    font-size: $H14;
    color: $ND6;
    margin-bottom: 68px;
    text-align: center;
    line-height: 1.75;
  }
  &__links-wrapper {
    display: flex;
  }
  &__links-wrapper .button:not(:last-child) {
    margin-right: 30px;
  }
  &__button {
    border: 1px solid $NL2;
    &:hover {
      background-color: $R1;
      border: 1px solid transparent;
    }
  }

  &__scroll-down {
    position: relative;
    z-index: 10;
    left: 50%;
    bottom: 84px;
    transform: translateX(-50%);
    display: flex;
    justify-content: center;
    align-items: center;
    img {
      z-index: 100;
    }
    &::after {
      content: "";
      position: absolute;
      min-width: 74px;
      min-height: 74px;
      background-color: $NL2;
      opacity: 0.25;
      border-radius: 50%;
    }
    &::before {
      content: "";
      position: absolute;
      min-width: 64px;
      min-height: 64px;
      background-color: $NL1;
      border-radius: 50%;
    }
  }
}
.slider-container {
  position: absolute;
  left: 0;
  top: 0;
  right: 0;
  bottom: 0;
  z-index: 1;
  min-width: 100%;
  min-height: 100vh;
}
.slider {
  min-width: 100%;
  min-height: 95vh;
}
.slider__item {
  min-width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}
.item1 {
  background: url(../img/header/background.png) center no-repeat;
  background-size: cover;
}
.item2 {
  background: url(../img/header/city.jpg) center no-repeat;
  background-size: cover;
}
.item3 {
  background: url(../img/header/city2.jpg) center no-repeat;
  background-size: cover;
}
.slidenav {
  position: relative;
  width: 45px;
  height: 45px;
  border-radius: 2px;
  background-color: $ND7;
  color: $ND3;
  font-size: $H36;
  display: flex;
  justify-content: center;
  align-items: center;
  &:hover {
    color: $NL2;
    background-color: $R1;
  }
}

.dots {
  position: absolute;
  right: 40px;
  top: 50%;
  transform: translateY(-50%);
  display: flex;
  flex-direction: column;
}
.dots li > a {
  border: 1px solid white;
}
.dots > li:not(:last-child) {
  margin-bottom: 40px;
  outline: none;
}
.dots .uk-active > a {
  background-color: white;
}

.uk-dotnav > * > :focus,
.uk-dotnav > * > :hover {
  background-color: transparent;
  outline: 0;
  border: 1px solid white;
}
.hamburger-menu {
  position: fixed;
  z-index: 10;
  width: 100%;
  height: 65px;
  &__title {
    position: absolute;
    top: 20px;
    right: 20px;
    position: fixed;
    font-size: $H22;
    color: $NL2;
    letter-spacing: 3px;
    line-height: 1.2;
  }

  @media screen and (min-width: 1023px) {
    display: none;
  }
}

#menu__toggle {
  opacity: 0;
}

#menu__toggle:checked ~ .menu__btn > span {
  transform: rotate(45deg);
}
#menu__toggle:checked ~ .menu__btn > span::before {
  top: 0;
  transform: rotate(0);
}
#menu__toggle:checked ~ .menu__btn > span::after {
  top: 0;
  transform: rotate(90deg);
}
#menu__toggle:checked ~ .menu__box {
  visibility: visible;
  left: 0;
}

.menu__btn {
  display: flex;
  align-items: center;
  position: fixed;
  top: 20px;
  left: 20px;

  width: 26px;
  height: 26px;

  cursor: pointer;
  z-index: 1;
}

.menu__btn > span,
.menu__btn > span::before,
.menu__btn > span::after {
  display: block;
  position: absolute;

  width: 100%;
  height: 2px;

  background-color: $NL2;

  transition-duration: 0.25s;
}
.menu__btn > span::before {
  content: "";
  top: -8px;
}
.menu__btn > span::after {
  content: "";
  top: 8px;
}

.menu__box {
  display: block;
  position: fixed;
  visibility: hidden;
  top: 0;
  left: -100%;

  width: 300px;
  height: 100%;
  max-height: 420px;

  margin: 0;
  padding: 80px 0;

  list-style: none;

  background-color: #eceff1;
  box-shadow: 1px 0px 6px rgba(0, 0, 0, 0.2);

  transition-duration: 0.25s;
}

.menu__item {
  display: block;
  padding: 12px 24px;

  color: #333;

  font-family: "Roboto", sans-serif;
  font-size: 20px;
  font-weight: 600;

  text-decoration: none;

  transition-duration: 0.25s;
}
.menu__item:hover {
  background-color: #cfd8dc;
}
.filled {
  transition: all 1s ease-in-out;
  background-color: rgba($color: #01183f, $alpha: 0.4);
}
</style>
