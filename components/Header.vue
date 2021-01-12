<template>
  <header class="w-full">
    <div class="container py-4 mx-auto px-5 flex items-center justify-between">
      <img class="h-20" src="@/assets/images/logo.png" alt="olonje" />
      <nav>
        <ul class="flex">
          <li class="pr-20 active"><a href="#">Home</a></li>
          <li class="pr-20"><a href="#">Product</a></li>
          <li class="pr-20"><a href="#">Faq</a></li>
          <li class=""><a href="#">Contact</a></li>
        </ul>

        <div class="hamburger">
          <div></div>
        </div>
      </nav>
    </div>
  </header>
</template>

<style lang="scss" scoped>
.active {
  color: #fa4a0c;
}

.hamburger {
  display: none;
  width: 30px;

  div,
  &::before,
  &::after {
    background-color: #737373;
    border-radius: 3px;
    content: '';
    display: block;
    height: 3px;
    margin: 5px 0;
  }

  @media screen and (max-width: 640px) {
    display: inline-block;
  }
}

img {
  @media screen and (max-width: 640px) {
    height: 50px;
  }
}

ul {
  @media screen and (max-width: 640px) {
    display: none;
  }
}
</style>
