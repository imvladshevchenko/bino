<template>
  <div class="footer">
    <div class="container">
      <ul class="footer__list">
        <li class="footer__item">
          <a href="#" class="footer__link"><i class="fab fa-facebook-f"></i></a>
        </li>
        <li class="footer__item">
          <a href="#" class="footer__link"><i class="fab fa-twitter"></i></a>
        </li>
        <li class="footer__item">
          <a href="#" class="footer__link"><i class="fas fa-rss"></i></a>
        </li>
        <li class="footer__item">
          <a href="#" class="footer__link"
            ><i class="fab fa-google-plus-g"></i
          ></a>
        </li>
        <li class="footer__item">
          <a href="#" class="footer__link"
            ><i class="fab fa-linkedin-in"></i
          ></a>
        </li>
        <li class="footer__item">
          <a href="#" class="footer__link"><i class="fab fa-skype"></i></a>
        </li>
        <li class="footer__item">
          <a href="#" class="footer__link"><i class="fab fa-vimeo-v"></i></a>
        </li>
        <li class="footer__item">
          <a href="#" class="footer__link"><i class="fab fa-tumblr"></i></a>
        </li>
      </ul>
      <p class="footer__rights">Kazi Erfan © All Rights Reserved</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "vue-footer",
};
</script>

<style lang="scss" >
.container {
  display: flex;
  justify-content: space-between;
}
$styles: footer;
.#{$styles} {
  padding-top: 35px;
  background-color: $ND2;
  &__list {
    display: flex;
  }
  &__item:not(:last-child) {
    margin-right: 25px;
  }
  &__item>* {
    color: rgb(153, 153, 153);
    font-size: $H20;
  }
  &__rights {
    font-family: $base-font;
    font-size: $H14;
    font-weight: 600;
    color: rgba(153, 153, 153, 0.75);
    margin-bottom: 35px;
  }
  &__link:hover {
    color: $R1;
    text-decoration: none;
  }
}
</style>
