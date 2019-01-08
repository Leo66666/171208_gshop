<template>
  <div id="App">
    <router-view/>

    <!-- 只有在当前路由不等于login的时候才显示footer -->
    <FooterGuide v-show="$route.meta.showFooter" />
  </div>
</template>
<script>
import FooterGuide from './components/FooterGuide/FooterGuide.vue'
export default {
  components: {
    FooterGuide
  }
}
</script>
<style lang="stylus" rel="stylesheet/stylus">
  .app
    width:100%
    height:100%
    background #f5f5f5
</style>
