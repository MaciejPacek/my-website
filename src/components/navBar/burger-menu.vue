<template>
    <div>
        <button class="burger-menu-button" @click="toggleMenu">
            <img src="../../assets/images/Sort.png"/>
        </button>
    </div>
    <div v-if="isOpen" class="mobile-menu">
      <!-- Treść menu -->
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Service</a></li>
        <li><a href="#">Contact</a></li>
        <li><a href="#">About me</a></li>
      </ul>
    </div>
</template>

<script>
    export default {
        name: 'BurgerMenu',
        data() {
            return {
                isOpen: true,
            }
        },
        mounted(){

        }
    }
</script>
<style lang="less" scoped>
  @import './burger-menu.less';
</style>