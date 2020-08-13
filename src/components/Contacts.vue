<template>
  <div class="contacts">
    <div class="container">
      <h2 class="title">KEEP IN TOUCH</h2>
      <p class="subtitle">
        Nullam sit amet odio eu est aliquet euismod a a urna. Proin eu urna
        suscipit, dictum quam nec.
      </p>
      <div class="dot-with-lines"></div>
      <div class="contacts__wrapper">
        <ul class="contacts__list">
          <li class="contacts__item">
            <p class="contacts__info">OUR ADDRESS</p>
            <a href="https://www.google.com/maps/place/%D0%A1%D0%B8%D0%B4%D0%BD%D0%B5%D0%B9%D1%81%D0%BA%D0%B8%D0%B9+%D0%BE%D0%BF%D0%B5%D1%80%D0%BD%D1%8B%D0%B9+%D1%82%D0%B5%D0%B0%D1%82%D1%80/@-33.860811,151.3038852,10.9z/data=!3m1!5s0x6b12ae67d234a27f:0xd6d4e9380ca1e32f!4m8!1m2!2m1!1sHouse+%2313,+Streat+road,+Sydney+2310+Australia!3m4!1s0x6b12ae665e892fdd:0x3133f8d75a1ac251!8m2!3d-33.8568028!4d151.2153053" class="contacts__subinfo">House #13, Streat road, Sydney 2310 Australia</a>
          </li>
          <li class="contacts__item">
            <p class="contacts__info">CALL US</p>
            <a href="tel:+ 880 168 109 1425" class="contacts__subinfo"
              >+ 880 168 109 1425</a
            >
            <a href="tel:+ 0216809142" class="contacts__subinfo"
              >+ 0216809142</a
            >
          </li>
          <li class="contacts__item">
            <p class="contacts__info">EMAIL US</p>
            <a href="mailto:contactus@email.com" class="contacts__subinfo"
              >contactus@email.com</a
            >
          </li>
        </ul>
        <form action="#" class="contacts__form">
          <input class="contacts__input" type="text" placeholder="Name" />
          <input class="contacts__input" type="text" placeholder="Email" />
          <input class="contacts__input" type="text" placeholder="Subject" />
          <textarea
            class="contacts__input contacts__textarea"
            cols="30"
            rows="7"
            placeholder="Message"
          ></textarea>
          <button class="contacts__button" type="submit">SEND MESSAGE</button>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "app",
};
</script>

<style lang="scss">
$styles: contacts;
.#{$styles} {
  padding-top: 150px;
  background-color: $NL1;
  .container {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  &__wrapper {
    display: flex;
    width: 100%;
    justify-content: space-between;
    margin-bottom: 152px;
  }
  &__list {
    padding: 99px 0 97px 91px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    flex-basis: 50%;
    max-width: 478px;
    background-color: $NL2;
    box-shadow: 0px 3px 5px 0 rgba(0, 0, 0, 0.1);
    border-radius: 2px;
    margin-right: 28px;
  }
  &__item:not(:last-child) {
    margin-bottom: 70px;
  }
  &__item {
    max-width: 270px;
    display: flex;
    flex-direction: column;
  }
  &__info {
    font-family: $sec-font;
    font-size: $H24;
    color: $R2;
    margin-bottom: 28px;
    font-weight: 600;
    line-height: 1;
  }
  &__subinfo {
    font-family: $base-font;
    font-size: $H18;
    color: $ND9;
    line-height: 1.33;
    &:hover {
      color: $ND9;
    }
  }
  &__form {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    flex-basis: 70%;
    max-width: 665px;
    background-color: $NL2;
    box-shadow: 0px 3px 5px 0 rgba(0, 0, 0, 0.1);
    border-radius: 2px;
    padding: 100px 50px 97px 102px;
  }
  &__input {
    padding-bottom: 19px;
    width: 100%;
    max-width: 464px;
    margin-bottom: 29px;
    border: none;
    border-bottom: 1px solid $ND9;
    font-family: $base-font;
    font-size: $H14;
    color: $ND9;
    font-weight: 600;
    outline: none;
    resize: none;
  }
  &__textarea {
    padding: 0;
    max-height: 115px;
    margin-bottom: 45px;
  }
  &__button {
    width: 100%;
    max-width: 157px;
    height: 44px;
    border-radius: 2.4px;
    box-shadow: 0px 2px 4.8px 0.3px rgba(0, 0, 0, 0.25);
    font-family: $base-font;
    font-size: $H14;
    color: $NL2;
    font-weight: bold;
    background-color: $ND9;
    border: none;
    transition: all 0.3s ease-in-out;
    outline: none;
    &:hover {
      background-color: $R1;
    }
  }
}
</style>
