<template>
<div class="header">
  <span>城市选择</span>
  <router-link to="/">
    <i class="iconfont header-back">&#xe611;</i>
  </router-link>
</div>
</template>

<script>
export default {
  name: 'CityHeader'
}
</script>

<style lang="stylus" scoped>
.header
  position relative
  overflow hidden
  height .86rem
  line-height .86rem
  text-align center
  color  #ffffff
  background #00bcd4
  font-size .32rem
  .header-back
    position absolute
    top 0
    left 0
    display block
    width .64rem
    text-align center
    font-size .4rem
    color #ffffff
</style>
