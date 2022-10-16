<template>
<swiper class="swiper-container">
  <div class="swiper-wrapper">
    <div class="swiper-slide">
      <img class="h-64 w-64" src="~assets/img/home/main-left.jpg" />
    </div>
    <div class="swiper-slide">
      <img class="h-64 w-64" src="~assets/img/home/main-right.jpg" />
    </div>
    <div class="swiper-slide">
      <img class="h-64 w-64" src="~assets/img/home/main-left.jpg" />
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
      slidesPerView: 2,
    })
  }
}
</script>

<style scoped lang="scss">
  img {
    max-width: 100%;
  }
</style>