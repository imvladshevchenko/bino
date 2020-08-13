<template>
  <div class="description">
    <div class="container">
      <ul class="description__list">
        <li class="description__item">
          <div class="description__icon-wrapper">
            <div class="description__icon-border"></div>
            <img class="description__img" src="../img/who-we-are/1.png" alt="icon" />
          </div>
          <h2 class="description__title">SLEEK DESIGN</h2>
          <p class="description__text">
            Lorem Ipsum is simply dummy text of the printing and typesetting
            let. Lorem Ipsum has been the industry.
          </p>
        </li>
        <li class="description__item">
          <div class="description__icon-wrapper">
            <div class="description__icon-border"></div>
            <img class="description__img" src="../img/who-we-are/2.png" alt="icon" />
          </div>
          <h2 class="description__title">CLEAN CODE</h2>
          <p class="description__text">
            Lorem Ipsum is simply dummy text of the printing and typesetting
            let. Lorem Ipsum has been the industry.
          </p>
        </li>
        <li class="description__item">
          <div class="description__icon-wrapper">
            <div class="description__icon-border"></div>
            <img class="description__img" src="../img/who-we-are/3.png" alt="icon" />
          </div>
          <h2 class="description__title">CREATIVE IDEAS</h2>
          <p class="description__text">
            Lorem Ipsum is simply dummy text of the printing and typesetting
            let. Lorem Ipsum has been the industry.
          </p>
        </li>
        <li class="description__item">
          <div class="description__icon-wrapper">
            <div class="description__icon-border"></div>            
            <img class="description__img" src="../img/who-we-are/4.png" alt="icon" />
          </div>
          <h2 class="description__title">FREE SUPPORT</h2>
          <p class="description__text">
            Lorem Ipsum is simply dummy text of the printing and typesetting
            let. Lorem Ipsum has been the industry.
          </p>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "Description",
};
</script>

<style lang="scss">
$styles: description;
.#{$styles} {
  padding-bottom: 112px;
  border-bottom: 1px solid $ND8;
  &__list {
    display: flex;
    align-items: center;
  }
}
</style>
