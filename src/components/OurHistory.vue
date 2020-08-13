<template>
  <div class="our-history">
    <div class="container">
      <div class="our-history__img-wrapper">
        <img src="../img/about-us/Monitor.png" alt="monitor" />
      </div>
      <div class="our-history__description">
        <h2 class="our-history__title">OUR HISTORY</h2>
        <div class="our-history__text-wrapper">
          <p class="our-history__text">
            Lorem Ipsum is simply dummy text of the printing and typesetting
            industry. Lorem Ip sum has been the industry's standard dummy text
            ever since the 1500s, when an unk- nown printer took a galley of
            type and scrambled it to make a type specimen book.
          </p>
          <p class="our-history__text">
            It has survived not only five centuries, but also the leap into
            electronic typesetting, remaining essentially unchanged. It was
            popularised in the 1960s with the release of Letraset sheets
            containing Lorem Ipsum passages, and more recently with desktop
            publishing software like Aldus PageMaker including versions of Lorem
            Ipsum.
          </p>
        </div>
        <a class="button our-history__button" href="">BROWSE OUR WORK</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "OurHistory",
};
</script>

<style lang="scss">
$styles: our-history;
.#{$styles} {
  padding: 141px 0 148px 0;
  .container {
    display: flex;
  }
  &__img-wrapper {
    margin-right: 77px;
    min-width: 506px;
    min-height: 407px;
    display: flex;
    align-items: center;
  }
  &__title {
    font-family: $sec-font;
    color: $ND4;
    font-size: $H36;
    letter-spacing: 3.6px;
    padding-left: 29px;
    border-left: 6px solid $R1;
    margin-bottom: 54px;
  }
  &__text {
    font-family: $sec-font;
    font-size: $H14;
    color: $ND9;
    line-height: 2.07;
    font-weight: normal;
  }
  &__text:not(:last-child) {
    margin-bottom: 25px;
  }
  &__text:last-child {
    margin-bottom: 47px;
  }
  &__button {
    background-color: $ND9;
       &:hover {
    background-color: $R1;
  }
  }
}
</style>
