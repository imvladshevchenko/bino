<template>
  <div class="our-pricing">
    <div class="container">
      <h2 class="title">OUR PRICING</h2>
      <p class="subtitle">
        A 30 days free trial for all. A brief story about how this process
        works, keep an eye till the end.
      </p>
      <div class="dot-with-lines"></div>
      <ul class="our-pricing__card">
        <li class="our-pricing__item">
          <p class="our-pricing__pack">STARTER</p>
          <div class="our-pricing__price-wrapper">
            <p class="our-pricing__price">$19</p>
            <span class="our-pricing__period">per month</span>
          </div>
          <div class="our-pricing__description-wrapper">
            <ul class="our-pricing__list">
              <li>
                <p class="our-pricing__text">Competition Analysis Methods</p>
              </li>
              <li>
                <p class="our-pricing__text">All Ranked URLs</p>
              </li>
              <li>
                <p class="our-pricing__text">International Support System</p>
              </li>
              <li>
                <p class="our-pricing__text">Social Media Tracking</p>
              </li>
            </ul>
            <a class="button our-pricing__button" href="#">CHOOSE PLAN</a>
          </div>
        </li>
        <li class="our-pricing__item">
          <p class="our-pricing__pack">PREMIUM</p>
          <div class="our-pricing__price-wrapper">
            <p class="our-pricing__price">$39</p>
            <span class="our-pricing__period">per month</span>
          </div>
          <div class="our-pricing__description-wrapper">
            <ul class="our-pricing__list">
              <li>
                <p class="our-pricing__text">Competition Analysis Methods</p>
              </li>
              <li>
                <p class="our-pricing__text">All Ranked URLs</p>
              </li>
              <li>
                <p class="our-pricing__text">International Support System</p>
              </li>
              <li>
                <p class="our-pricing__text">Social Media Tracking</p>
              </li>
            </ul>
            <a class="button our-pricing__button" href="#">CHOOSE PLAN</a>
          </div>
        </li>
        <li class="our-pricing__item">
          <p class="our-pricing__pack">BUSINESS</p>
          <div class="our-pricing__price-wrapper">
            <p class="our-pricing__price">$99</p>
            <span class="our-pricing__period">per month</span>
          </div>
          <div class="our-pricing__description-wrapper">
            <ul class="our-pricing__list">
              <li>
                <p class="our-pricing__text">Competition Analysis Methods</p>
              </li>
              <li>
                <p class="our-pricing__text">All Ranked URLs</p>
              </li>
              <li>
                <p class="our-pricing__text">International Support System</p>
              </li>
              <li>
                <p class="our-pricing__text">Social Media Tracking</p>
              </li>
            </ul>
            <a class="button our-pricing__button" href="#">CHOOSE PLAN</a>
          </div>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "OurPricing",
};
</script>

<style lang="scss">
$styles: our-pricing;
.#{$styles} {
  padding: 156px 0 143px 0;
  .container {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  &__card {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    width: 100%;
    
        @media screen and (min-width: 1025px) {
      justify-content: space-between;
      }
  }
  &__item {
    position: relative;
    display: flex;
    flex-direction: column;
    background-color: $ND9;
    padding-top: 50px;
    flex-basis: 50%;
    max-width: 360px;
    align-items: center;
    transition: all 0.3s ease-in-out;
    @media screen and (min-width: 1025px) {
      &:hover {
        background-color: $R1;
        flex-basis: 35%;
    max-width: 360px;
      }
    }
  }
  &__item:nth-of-type(1) {
    margin-right: 30px;
    @media screen and (min-width: 1199px) {
      margin: 0;
    }
  }
  &__item:not(:last-child) {
    margin-bottom: 30px;
    @media screen and (min-width: 1199px) {
      margin: 0;
    }
  }
  &__pack {
    font-family: $base-font;
    font-size: $H24;
    font-weight: 600;
    color: $NL2;
    letter-spacing: 1.8px;
    margin-bottom: 136px;
  }
  &__price-wrapper {
    position: absolute;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    top: 178px;
    z-index: 10;
    &::after {
      content: "";
      position: absolute;
      min-width: 174px;
      min-height: 174px;
      background-color: $NL2;
      opacity: 0.25;
      border-radius: 50%;
    }
    &::before {
      content: "";
      position: absolute;
      min-width: 154px;
      min-height: 154px;
      background-color: $NL1;
      border-radius: 50%;
    }
  }
  &__price {
    font-family: $sec-font;
    font-size: $H40;
    color: $ND9;
    font-weight: bold;
    margin-bottom: 6px;
    z-index: 100;
  }
  &__period {
    font-family: $sec-font;
    font-size: $H13;
    color: $ND9;
    z-index: 100;
  }
  &__description-wrapper {
    background-color: $NL1;
    padding-top: 125px;
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 100%;
  }
  &__list {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-bottom: 48px;
  }
  &__list > * {
    font-family: $base-font;
    font-size: $H14;
    color: $ND9;
    font-weight: 600;
  }
  &__list > *:not(:last-child) {
    margin-bottom: 40px;
  }
  &__button {
    background-color: $ND9;
    margin-bottom: 50px;
    &:hover {
      background-color: $R1;
    }
  }
}
</style>
