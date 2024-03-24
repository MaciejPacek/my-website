<template>
   <div class="main">
      <NavBar/>
      <div class="background-gradient"></div>
      <img class="image" src="./assets/images/background-img.png" alt="">
   </div>
</template>

<script>
import NavBar from './components/navBar/navBar.vue'
export default {
  name: 'App',
  components: {
    NavBar,
  }
}
</script>


<style lang="less" scoped>
  @import './assets/css/main.less';
</style>

