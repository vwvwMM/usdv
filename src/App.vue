<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
import {bootstrapWidget, themes} from '@usdv/usdv-widget'

bootstrapWidget({
  color: 22,
  theme: themes.light  
})
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="https://i0.wp.com/coocolab.com/wp-content/uploads/2019/10/cropped-%E9%85%B7%E5%8F%AF%E5%AF%A6%E9%A9%97%E5%AE%A4logo-%E7%99%BD%E9%82%8A.png?fit=250%2C100&ssl=1" height="125" />

    <!-- <div class="wrapper">
      <HelloWorld msg="You did it!" />
    </div> -->
  </header>

  <main>
    <usdv-widget style="padding:20px"></usdv-widget>
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
