<template>
<div class="wrapper">
  <swiper :options="swiperOptions" v-if="showSwiper">
    <swiper-slide v-for="item in list" :key="item.id">
      <img class="swiper-img" :src="item.imgUrl">
    </swiper-slide>
    <div class="swiper-pagination" slot="pagination"></div>
  </swiper>
</div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  props: {
    list: Array
  },
  data () {
    return {
      swiperOptions: {
        pagination: '.swiper-pagination',
        loop: true
      }
    }
  },
  computed: {
    showSwiper () {
      return this.list.length
    }
  }
}
</script>

<style lang="stylus" scoped>
.wrapper >>> .swiper-pagination-bullet-active
    background: #ffffff
.wrapper
  width: 100%
  height: 0
  overflow: hidden
  padding-bottom: 31.25%
  background: #eeeeee
  .swiper-img
    width: 100%
</style>
