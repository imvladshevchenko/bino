<template>
  <div class="free-trial">
    <div class="container">
      <h2 class="free-trial__title">Let's Get Started Now. <span>It's FREE!</span></h2>
      <p class="free-trial__text">
        30 day free trial. Free plan allows up to 2 projects. Pay if you need
        more. Cancel anytime. No catches.
      </p>
      <a class="button free-trial__button" href="#">start free trial</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "FreeTrial",
};
</script>

<style lang="scss" scooped>
$styles: free-trial;
.#{$styles} {
  padding-top: 150px;
  background: url(../img/promo/Background.png) center center;
  background-size: cover;
  .container {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  &__title {
    font-family: $base-font;
    font-size: $H36;
    text-align: center;
    color: $NL2;
    margin-bottom: 15px;
  }
  &__title>span {
    font-weight: bold;
  }
  &__text {
    font-family: $base-font;
    font-size: $H18;
    color: $NL2;
    text-align: center;
    margin-bottom: 70px;
  }
  &__button {
    border: 1px solid $NL2;
    margin-bottom: 140px;
      &:hover {
    background-color: $R1;
    border: 1px solid transparent;
  }
  }
}
</style>
