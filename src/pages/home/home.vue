<template>
    <div class="home">
      <home-header></home-header>
      <home-swiper></home-swiper>
      <p>123</p>
    </div>
</template>
<script>
import HomeHeader from './components/header'
import HomeSwiper from './components/swiper'
export default {
  name: 'Home',
  data () {
    return {}
  },
  components: { HomeHeader, HomeSwiper }

}
</script>

<style lang="less" scoped>

</style>


