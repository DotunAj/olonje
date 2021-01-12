<template>
  <div class="">
    <section class="w-full flex">
      <div class="container flex items-center justify-center flex-col mx-auto">
        <h1
          class="text-5xl xl:w-2/3 w-full text-center text-white font-bold mt-5"
        >
          Download the app now.
        </h1>
        <!-- <p class="text-xl text-gray-400 text-center mt-5 font-medium">
        Download the bella onoje’s food app now on
      </p> -->

        <div class="flex md:flex-row flex-col mt-5">
          <button class="button__primary md:mr-6">Playstore</button>
          <button class="button__secondary md:mt-0 mt-6">App store</button>
        </div>
      </div>
    </section>

    <footer>
      <div
        class="container py-4 mx-auto px-5 flex md:flex-row flex-col items-center justify-between"
      >
        <img class="h-20" src="@/assets/images/logo.png" alt="olonje" />
        <nav>
          <ul class="flex items-center">
            <li class="pr-5 active">
              <a href="#"><TwitterIcon /></a>
            </li>
            <li class="pr-5 active">
              <a href="#"><FacebookIcon /></a>
            </li>
            <li class="pr-5 active">
              <a href="#"><InstagramIcon /></a>
            </li>
          </ul>
        </nav>
        <span class="text-gray-700 text-sm md:mt-0 mt-5"
          >Copywright 2020 Bella Onojie.com</span
        >
      </div>
    </footer>
  </div>
</template>

<style lang="scss" scoped>
section {
  margin-top: 50px;
  @media screen and (min-width: 640px) {
    background: url('~assets/images/hero-b.png');
    background-size: cover;
    min-height: 419px;
  }
  background-color: #252b42;
  padding: 20px;

  h1 {
    font-family: 'Poppins', sans-serif;
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
      /* @media screen and (max-width: 640px) {
        border: 1px solid #fa4a0c;
        color: #fa4a0c;
      } */
      background: transparent;
      border: 1px solid #fff;
      &:hover {
        box-shadow: 0px 10px 30px rgba(183, 51, 39, 0.356);
      }
    }
  }
}

footer {
  img {
    @media screen and (max-width: 640px) {
      display: none;
    }
  }
}
</style>
