<template>
  <section class="container">
    <div>
       <ul>
      <li><nuxt-link :to="{name:'index'}">HOME</nuxt-link></li>
      <li><nuxt-link :to="{name:'about'}">ABOUT</nuxt-link></li>
      <li><nuxt-link :to="{name:'news',params:{newsId:222}}">NEWS</nuxt-link></li>
      <li><nuxt-link :to="{name:'asyncData'}">asyncData</nuxt-link></li>
    </ul>
    <div>
      <img src="~static/timg.jpg" alt="">
    </div>
    </div>
  </section>
</template>

<script>
import AppLogo from '~/components/AppLogo.vue'

export default {
  components: {
    AppLogo
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
