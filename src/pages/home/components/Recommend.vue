<template>
<div>
  <div class="title">热销推荐</div>
  <ul>
    <li class="item" v-for="item in recommendList" :key="item.id">
      <img class="item-img" :src="item.imgUrl">
      <div class="item-info border-bottom">
        <p class="item-title">{{item.title}}</p>
        <p class="item-desc">{{item.desc}}</p>
        <button class="item-buttton">查看详情</button>
      </div>
    </li>
  </ul>

</div>
</template>

<script>
export default {
  name: 'HomeRecommend',
  data () {
    return {
      recommendList: [{
        id: '0001',
        imgUrl: 'https://imgs.qunarzz.com/p/p27/201302/28/d14185ac8a47f6f993835fbb.jpg_256x160_c2ab9336.jpg',
        title: '阿迪回哦啊',
        desc: '阿迪后期而为i哦发热温暖'
      }, {
        id: '0002',
        imgUrl: 'https://imgs.qunarzz.com/p/p27/201302/28/d14185ac8a47f6f993835fbb.jpg_256x160_c2ab9336.jpg',
        title: '阿迪回哦啊',
        desc: '阿迪后期而为i哦发热温暖'
      }, {
        id: '0003',
        imgUrl: 'https://imgs.qunarzz.com/p/p27/201302/28/d14185ac8a47f6f993835fbb.jpg_256x160_c2ab9336.jpg',
        title: '阿迪回哦啊',
        desc: '阿迪后期而为i哦发热温暖'
      }, {
        id: '0004',
        imgUrl: 'https://imgs.qunarzz.com/p/p27/201302/28/d14185ac8a47f6f993835fbb.jpg_256x160_c2ab9336.jpg',
        title: '阿迪回哦啊',
        desc: '阿迪后期而为i哦发热温暖'
      }]
    }
  }
}
</script>

<style lang="stylus" scoped>
.title
  margin-top .2rem
  line-height .8rem
  background #eeeeee
  text-indent .2rem
.item
  display flex
  height 1.9rem
  overflow hidden
  .item-img
    width 1.7rem
    height 1.7rem
    padding .1rem
  .item-info
    flex 1
    padding .1rem
    .item-title
      line-height .54rem
      font-size  .32rem
    .item-desc
      line-height .4rem
      color #cccccc
    .item-buttton
      margin-top .2rem
      line-height .44rem
      color #ffffff
      background  #ff9300
      padding  0 .1rem
      border-radius .06rem
</style>
