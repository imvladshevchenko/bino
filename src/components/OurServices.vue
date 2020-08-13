<template>
  <div class="our-services">
    <h2 class="our-services__title"></h2>
    <div
      class="uk-position-relative uk-visible-toggle uk-light our-services__slider-wrapper"
      tabindex="-1"
      uk-slider
    >
      <ul
        class="uk-slider-items uk-child-width-1-2 uk-child-width-1-3@m uk-grid our-services__slider-list"
      >
        <li class="our-services__slider-item">
          <div class="uk-panel">
            <h4 class="our-services__item-subtitle"></h4>
            <p class="our-services__text"></p>
            <img src="../img/services/Forma1.png" alt="icon" />
          </div>
        </li>
        <li class="our-services__slider-item">
          <div class="uk-panel">
            <h4 class="our-services__item-subtitle"></h4>
            <p class="our-services__text"></p>
            <img src="../img/services/Forma2.png" alt="icon" />
          </div>
        </li>
        <li class="our-services__slider-item">
          <div class="uk-panel">
            <h4 class="our-services__item-subtitle"></h4>
            <p class="our-services__text"></p>
            <img src="../img/services/Forma3.png" alt="icon" />
          </div>
        </li>
      </ul>
      <ul class="uk-slider-nav uk-dotnav"></ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "OurServices",
};
</script>

<style lang="scss"></style>
