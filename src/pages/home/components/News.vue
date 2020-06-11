<template>
<div class="container">
  <textarea v-model="message" placeholder="add multiple lines"></textarea>
  <p>这是用户输入的原始数据: {{message}} </p>

  <p>下面是转义的数据</p>
  <div v-html="showMessage" class="message-father"></div>
</div>
</template>

<script>
export default {
  name: 'News',
  data () {
    return {
      message: ''
    }
  },
  computed: {
    showMessage () {
      return `<div class="div-message">${this.message}</div>`
    }
  }
}
</script>

<style lang="stylus" scoped>
.container >>> .div-message
  color red
</style>
