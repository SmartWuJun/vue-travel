<template>
    <div class="header">
      <div class="header-left icon icon-back"></div>
      <div class="header-center icon icon-search">景点/目的地/主题</div>
      <div class="header-right">
        城市
        <i class="icon icon-arrowdown"></i>
      </div>
    </div>
</template>

<script>
export default {
  name: 'HomeHeader',
  data () {
    return {}
  }
}
</script>

<style lang="less" scoped>
.header {
  background: #00bcd4;
  height: 90px;
  display: flex;
  align-items: center;
  color: #fff;
  .header-left {
    width: 80px;
    padding-left: 20px;
    font-size: 36px;
  }
  .header-center {
    flex: 1;
    border-radius: 4px;
    background: #fff;
    color: #ccc;
    font-size: 28px;
    height: 60px;
    line-height: 60px;
    padding-left: 20px;
  }
  .header-right {
    padding: 0 20px;
  }
}
</style>


