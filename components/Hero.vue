<template>
  <section class="w-full">
    <div class="container flex items-center justify-center flex-col mx-auto">
      <p class="md:text-lg text-sm md:text-white text-grey font-bold md:mt-20">
        Food app
      </p>
      <h1
        class="md:text-5xl text-3xl xl:w-2/3 w-full text-center md:text-white text-dark font-bold mt-5"
      >
        Why stay hungry when you can order form Bella Onojie
      </h1>
      <p class="text-xl text-grey mt-5 font-medium">
        Download the bella onoje’s food app now on
      </p>

      <div class="flex md:flex-row flex-col mt-5">
        <button class="button__primary md:mr-6">Playstore</button>
        <button class="button__secondary md:mt-0 mt-6">App store</button>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
section {
  @media screen and (min-width: 640px) {
    background: url('~assets/images/hero.png');
    background-size: cover;
    min-height: 619px;
  }
  background-color: #fafafa;
  padding: 20px;

  h1 {
    font-family: 'Poppins', sans-serif;
  }

  .text-grey {
    color: #737373;
    padding: 0 10px;
    text-align: center;
    @media screen and (min-width: 640px) {
      color: #f7f7f7;
    }
  }

  .text-dark {
    @media screen and (man-width: 640px) {
      color: #252b42;
    }
  }

  button,
  .button {
    transition-duration: 0.5s;
    border-radius: 30px;
    height: 68px;
    padding: 16px 50px;
    font-size: 1.1em;
    font-weight: bold;
    color: #fff;

    &__primary {
      background: #fa4a0c;
      &:hover {
        background-color: lighten($color: #fa4a0c, $amount: 2);
      }
    }

    &__secondary {
      @media screen and (max-width: 640px) {
        border: 1px solid #fa4a0c;
        color: #fa4a0c;
      }
      background: transparent;
      border: 1px solid #fff;
      &:hover {
        box-shadow: 0px 10px 30px rgba(183, 51, 39, 0.356);
      }
    }
  }
}
</style>
