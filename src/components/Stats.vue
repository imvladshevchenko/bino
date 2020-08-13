<template>
  <div class="stats">
    <div class="container">
      <ul class="stats__list">
        <li class="stats__item">
          <div class="stats__icon-wrapper">
            <img src="../img/stats/icon1.png" alt="icon" />
          </div>
          <p class="stats__stat">3891</p>
          <p class="stats__stat-description">User Favourites</p>
        </li>
        <li class="stats__item">
          <div class="stats__icon-wrapper">
            <img src="../img/stats/icon2.png" alt="icon" />
          </div>
          <p class="stats__stat">281K</p>
          <p class="stats__stat-description">Posts Last 24 Hours</p>
        </li>
        <li class="stats__item">
          <div class="stats__icon-wrapper">
            <img src="../img/stats/icon3.png" alt="icon" />
          </div>
          <p class="stats__stat">618</p>
          <p class="stats__stat-description">Total Posts</p>
        </li>
        <li class="stats__item">
          <div class="stats__icon-wrapper">
            <img src="../img/stats/icon4.png" alt="icon" />
          </div>
          <p class="stats__stat">178</p>
          <p class="stats__stat-description">Campaigns</p>
        </li>
        <li class="stats__item">
          <div class="stats__icon-wrapper">
            <img src="../img/stats/icon5.png" alt="icon" />
          </div>
          <p class="stats__stat">285</p>
          <p class="stats__stat-description">Amazing Features</p>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "Stats",
};
</script>

<style lang="scss">
$styles: stats;
.#{$styles} {
  padding: 155px 0 142px 0;
  background: url(../img/stats/Background.png) center no-repeat;
  background-size: cover;
  &__list {
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 100%;
  }
  &__item {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  &__icon-wrapper {
    min-width: 111px;
    min-height: 111px;
    display: flex;
    justify-content: center;
    align-items: center;
    border: solid 1px $NL2;
    border-radius: 50%;
    margin-bottom: 50px;
  }
  &__stat {
    font-family: $sec-font;
    font-size: $H30;
    font-weight: bold;
    color: $NL1;
    letter-spacing: 1.5px;
    margin-bottom: 10px;
  }
  &__stat-description {
    font-family: $sec-font;
    font-size: $H18;
    color: $NL1;
    letter-spacing: 0.9px;
  }
}
</style>
