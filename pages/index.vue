<template>
  <div class="home">
    <Hero />
    <div class="img-container">
      <img src="@/assets/images/phones.png" alt="" />
    </div>
    <div
      class="home__content container mx-auto flex flex-col mt-20 items-center"
    >
      <h1 class="md:w-1/2 md:text-4xl text-2xl font-bold flex justify-center">
        How the app works
      </h1>

      <div
        class="flex md:flex-row md:mt-20 flex-col items-center text-center px-10 md:w-10/12"
      >
        <div class="my-10 md:order-2 md:text-left">
          <p class="font-bold my-3 text-lg text-orange">Create an account</p>
          <h2 class="font-bold my-3 text-4xl text-dark">
            Create/login to an existing account to get started
          </h2>
          <p class="text-gray">
            An account is created with your email and a desired password
          </p>
        </div>

        <div class="md:w-1/2 md:mr-40">
          <img src="@/assets/images/phone1.png" alt="" />
        </div>
      </div>

      <div
        class="flex md:flex-row md:mt-20 flex-col items-center text-center px-10 md:w-10/12"
      >
        <div class="my-10 md:text-left">
          <p class="font-bold my-3 text-lg text-orange">
            Explore while shopping
          </p>
          <h2 class="font-bold my-3 text-4xl text-dark">
            Shop for your favorites meal as e dey hot.
          </h2>
          <p class="text-gray">
            Shop for your favorite meals or drinks and enjoy while doing it.
          </p>
        </div>

        <div class="md:w-1/2 md:ml-40">
          <img src="@/assets/images/phone2.png" alt="" />
        </div>
      </div>

      <div
        class="flex md:flex-row md:mt-20 flex-col items-center text-center px-10 md:w-10/12"
      >
        <div class="md:order-2 my-10 md:text-left">
          <p class="font-bold my-3 text-lg text-orange">
            Explore while shopping
          </p>
          <h2 class="font-bold my-3 text-4xl text-dark">
            Shop for your favorites meal as e dey hot.
          </h2>
          <p class="text-gray">
            Shop for your favorite meals or drinks and enjoy while doing it.
          </p>
        </div>

        <div class="md:w-1/2 md:mr-40 mr-3">
          <img src="@/assets/images/phone3.png" alt="" />
        </div>
      </div>
    </div>
    <HerolikeFooter />
  </div>
</template>

<script>
export default {}
</script>
<style lang="scss" scoped>
// HOME STYLE
.home {
  @media screen and (max-width: 640px) {
    background-color: #fafafa;
  }
  position: relative;
  .img-container {
    @media screen and (max-width: 640px) {
      top: 490px;
    }
    width: 100%;
    display: flex;
    flex-direction: column;
    align-self: center;
    justify-content: center;
    position: absolute;
    top: 450px;

    img {
      z-index: 0;
      @media screen and (max-width: 640px) {
        max-height: 400px;
      }
      object-fit: contain;
    }
  }

  &__content {
    @media screen and (max-width: 884px) {
      margin-top: 450px;
    }
    margin-top: 500px;
    position: relative;

    &::before {
      position: absolute;
      top: 0;
      content: '';
      height: 3px;
      width: 884px;
      background-color: #e4e4e4;

      @media screen and (max-width: 884px) {
        display: none;
      }
    }
    h1 {
      margin-top: 72px;

      @media screen and (max-width: 884px) {
        margin-top: 0px;
      }
    }
  }

  // TEXT UTILITIES

  .text-orange {
    color: #fa4a0c;
  }

  .text-dark {
    color: #252b42;
  }

  .text-gray {
    color: #737373;
  }
}
</style>
