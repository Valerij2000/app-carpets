<template>
<swiper class="swiper-container">
  <div class="swiper-wrapper">
    <div class="swiper-slide slide">
      <div class="slide__wrapper">
        <img class="slide__img" src="~assets/img/home/carusel/slide01.png" />
        <div class="slide__content">
          <h2 class="slide__title">
            <b class="slide__orange">Ковровые изделия</b> для <span class="nowrap">Вашего дома <span class="slide__point">.</span></span>
          </h2>
          <button class="slide__button">Открыть каталог</button>
        </div>
      </div>
    </div>
  </div>
</swiper>
</template>

<script>
import Swiper from 'swiper';
export default {
  name: 'Slider',
  mounted: function () {
    new Swiper('.swiper-container', {
      autoplay: true,
      loop: true,
      slidesPerView: 1,
    })
  }
}
</script>

<style lang="scss">
@import '~assets/scss/partials/mixins';
@import '~assets/scss/partials/var-colors';

.slide {
  &__img {
    @include img(cover);
    max-width: 750px;
  }

  &__wrapper {
    display: grid;
    grid-auto-flow: column;
    justify-content: space-between;
    align-items: center;
  }

  &__content {
    max-width: 600px;
  }

  &__title {
    font-family: 'Federo';
    font-style: normal;
    font-weight: 400;
    font-size: 80px;
    line-height: 90px;
    letter-spacing: 0.02em;
    color: $blackColor060;
    margin-bottom: 40px;
  }

  &__button {
    display: inline-flex;
    justify-content: center;
    align-items: center;
    background: #3A3A3A;
    ;
    padding: 8px 16px;
    font-weight: 400;
    font-size: 16px;
    line-height: 22px;
    letter-spacing: -0.035em;
    text-align: center;
    color: $whiteColor;
  }

  &__point {
    font-size: 90px;
    display: inline-block;
    border-radius: 50%;
    color: $redColor;
  }

  &__orange {
    color: $redColor;
    font-weight: 800;
  }
}
</style>
