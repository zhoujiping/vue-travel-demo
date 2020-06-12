<template>
<div class="header">
  <div class="header-left">
    <i class="iconfont back-icon">&#xe611;</i>
  </div>
  <div class="header-input">
    <i class="iconfont">&#xe60c;</i>
    <span>输入城市/景点/游玩主题</span>
  </div>
  <router-link to="/city">
    <div class="header-right">
      <span>{{this.city}}</span>
      <i class="iconfont arrow-icon">&#xe615;</i>
    </div>
  </router-link>
</div>
</template>

<script>
export default {
  name: 'HomeHeader',
  props: {
    city: String
  }
}
</script>

<style lang="stylus" scoped>
@import '~@/assets/styles/varibles.styl'
.header
  display: flex
  height: .86rem
  line-height: .86rem
  background: $bgColor
  color: #ffffff
  .header-left
    width: .64rem
    float: left
    .back-icon
      display: block
      text-align: center
      font-size: .4 rem
  .header-input
    flex: 1
    margin-top .12rem
    margin-left .2rem
    height: .64rem
    line-height .64rem
    background: #ffffff
    border-radius: .1rem
    color: #cccccc
    padding-left .1rem
  .header-right
    width: 1.24rem
    float: right
    text-align: center
    color #ffffff
    .arrow-icon
      font-size: .2rem
</style>
