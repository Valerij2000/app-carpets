<template>
<section class="main">
  <div class="main__wrapper">
    <div class="container">
      <h1 class="main__title">
        <b class="main__orange">Ковровые Изделия</b> Вашей мечты<span class="main__point">.</span>
      </h1>
      <p class="main__description">
        Новая коллекция ковров от Merinos
      </p>
      <Slider />
    </div>
  </div>
</section>
</template>

<style lang="scss" scoped>
@import '~assets/scss/partials/var-colors';

.main {
  &__wrapper {
    background-color: #F6F6F6;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 750px;
  }

  &__title {
    font-family: 'Federo';
    font-weight: 500;
    font-size: 60px;
    line-height: 120%;
    text-align: center;
    color: $blackColor060;
  }

  &__description {
    font-family: 'Federo';
    font-weight: 400;
    font-size: 20px;
    line-height: 140%;
    text-align: center;
    color: $greyColor888;
  }

  &__point {
    font-size: 80px;
    color: $redColor;
  }

  &__orange {
    color: $redColor;
    font-weight: 800;
  }
}
</style>
