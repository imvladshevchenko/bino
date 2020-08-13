<template>
  <div class="our-blog">
    <div class="our-blog__container">
      <h2 class="title">OUR BLOG</h2>
      <p class="subtitle">
        Suspendisse sed eros mollis, tincidunt felis eget, interdum eratullam
        sit amet odio.
      </p>
      <div class="dot-with-lines"></div>
      <ul class="our-blog__list">
        <li class="our-blog__img-item">
          <img src="../img/blog/1.png" alt="img" />
        </li>
        <li class="our-blog__description">
          <p class="our-blog__item-subtitle">art / t-shirt</p>
          <h6 class="our-blog__item-title">T-SHIRT DESIGN</h6>
          <p class="our-blog__item-text">
            Lorem Ipsum is simply dummy text of the printing and typesetting
            industry. Lorem Ipsum has been the indu Stry's standard dummy text
            ever since the 1500s, an unknown printer took a galley of type a
            scrambled it to make a type specimen book.
          </p>
          <a class="our-blog__item-link" href=""
            >Read More <i class="fas fa-angle-double-right"></i
          ></a>
        </li>
        <li class="our-blog__img-item">
          <img src="../img/blog/2.png" alt="img" />
        </li>
        <li class="our-blog__description">
          <p class="our-blog__item-subtitle">art / t-shirt</p>
          <h6 class="our-blog__item-title">T-SHIRT DESIGN</h6>
          <p class="our-blog__item-text">
            Lorem Ipsum is simply dummy text of the printing and typesetting
            industry. Lorem Ipsum has been the indu Stry's standard dummy text
            ever since the 1500s, an unknown printer took a galley of type a
            scrambled it to make a type specimen book.
          </p>
          <a class="our-blog__item-link" href=""
            >Read More <i class="fas fa-angle-double-right"></i
          ></a>
        </li>
        <li class="our-blog__description">
          <p class="our-blog__item-subtitle">art / t-shirt</p>
          <h6 class="our-blog__item-title">T-SHIRT DESIGN</h6>
          <p class="our-blog__item-text">
            Lorem Ipsum is simply dummy text of the printing and typesetting
            industry. Lorem Ipsum has been the indu Stry's standard dummy text
            ever since the 1500s, an unknown printer took a galley of type a
            scrambled it to make a type specimen book.
          </p>
          <a class="our-blog__item-link" href=""
            >Read More <i class="fas fa-angle-double-right"></i
          ></a>
        </li>
        <li class="our-blog__img-item">
          <img src="../img/blog/3.png" alt="img" />
        </li>
        <li class="our-blog__description">
          <p class="our-blog__item-subtitle">art / t-shirt</p>
          <h6 class="our-blog__item-title">T-SHIRT DESIGN</h6>
          <p class="our-blog__item-text">
            Lorem Ipsum is simply dummy text of the printing and typesetting
            industry. Lorem Ipsum has been the indu Stry's standard dummy text
            ever since the 1500s, an unknown printer took a galley of type a
            scrambled it to make a type specimen book.
          </p>
          <a class="our-blog__item-link" href=""
            >Read More <i class="fas fa-angle-double-right"></i
          ></a>
        </li>
        <li class="our-blog__img-item">
          <img src="../img/blog/4.png" alt="img" />
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: "OurBlog",
};
</script>

<style lang="scss">
$styles: our-blog;
.#{$styles} {
  padding-top: 120px;
  background-color: $NL1;
  display: flex;
  justify-content: center;
  &__container {
    max-width: 1920px;
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  &__list {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
  }
  &__list > * {
    max-width: 480px;
  }
  &__description {
    position: relative;
    background-color: $R2;
    padding: 71px 50px 0 50px;
    display: flex;
    flex-direction: column;
  }
  &__description:nth-child(2)::before {
    content: "";
    position: absolute;
    top: 50%;
    left: -28px;
    transform: translateY(-50%);
    border-style: solid;
    border-width: 35px 28px 35px 0;
    border-color: transparent #e74f3e transparent transparent;
  }
  &__description:nth-child(4)::before {
    content: "";
    position: absolute;
    top: 50%;
    left: -28px;
    transform: translateY(-50%);
    border-style: solid;
    border-width: 35px 28px 35px 0;
    border-color: transparent #e74f3e transparent transparent;
  }
  &__description:nth-child(5)::after {
    content: "";
    position: absolute;
    top: 50%;
    right: -28px;
    transform: translateY(-50%);
    border-style: solid;
    border-width: 35px 0 35px 28px;
    border-color: transparent transparent transparent #e74f3e;
  }
  &__description:nth-child(7)::after {
    content: "";
    position: absolute;
    top: 50%;
    right: -28px;
    transform: translateY(-50%);
    border-style: solid;
    border-width: 35px 0 35px 28px;
    border-color: transparent transparent transparent #e74f3e;
  }
  &__item-subtitle {
    font-family: $base-font;
    font-size: $H14;
    color: $NL2;
    letter-spacing: 0.7px;
    margin-bottom: 32px;
  }
  &__item-title {
    position: relative;
    font-family: $sec-font;
    font-weight: 600;
    font-size: $H24;
    letter-spacing: 1.2px;
    color: $NL2;
    margin-bottom: 70px;
    &::after {
      content: "";
      position: absolute;
      width: 44px;
      height: 4px;
      background-color: $NL2;
      top: 45px;
      left: 0;
    }
  }
  &__item-text {
    font-family: $base-font;
    font-size: $H16;
    line-height: 1.88;
    color: $NL2;
    margin-bottom: 50px;
  }
  &__item-link {
    font-family: $base-font;
    font-size: $H18;
    color: $NL2;
    font-weight: 600;
    font-style: italic;
  }
}
</style>
