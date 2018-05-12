<template>
  <swiper :options="swiperOption" ref="mySwiper" >
    <!-- slides -->
    <swiper-slide>
      <div class="img-box">
        <img src="https://imgs.qunarzz.com/piao/fusion/1804/bd/8e4a1c3f470d3702.jpg_640x170_c1e8baeb.jpg" alt="">
      </div>
    </swiper-slide>
    <swiper-slide>
      <div class="img-box">
        <img src="https://imgs.qunarzz.com/piao/fusion/1804/5c/969bfa7af00a2702.jpg_640x170_ec465291.jpg" alt="">
      </div>
    </swiper-slide>
   
    <!-- Optional controls -->
    <div class="swiper-pagination"  slot="pagination"></div>
  </swiper>
</template>
 
<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        // some swiper options/callbacks
        // 所有的参数同 swiper 官方 api 参数
        // ...
        pagination: {
          el: '.swiper-pagination'
        },
        loop: true
      }
    }
  },
  computed: {
    swiper () {
      return this.$refs.mySwiper.swiper
    }
  },
  mounted () {
    // current swiper instance
    // 然后你就可以使用当前上下文内的swiper对象去做你想做的事了
    console.log('this is current swiper instance object', this.swiper)
    //this.swiper.slideTo(3, 1000, false)
  }
}
</script>

<style lang="less" scoped>
.swiper-container /deep/ .swiper-pagination-bullet-active {
  background: #fff;
}
.img-box {
  height: 0;
  overflow: hidden;
  width: 100%;
  padding-bottom: 26.5%;
  img {
    width: 100%;
  }
}
</style>
