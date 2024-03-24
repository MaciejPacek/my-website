<template>
    <div class="navigation">
        <div class="navigation-frame-3" :class="{'active': active}">
            <img class="logo-img" src="../../assets/images/Logo11.png"/>
            <div class="navigation-group-3" >
                <div class="navigation-group-3-item">Home</div>
                <div class="navigation-group-3-item">Service</div>
                <div class="navigation-group-3-item">Contact</div>
                <div class="navigation-group-3-item">About me</div>
            </div>
            <div class="navigation-group-2">
                <div class="button-login"><span>Log in</span></div>
                <div class="button-sing-up"><span>Sing Up</span></div>
            </div>
        </div>
        <BurgerMenu />
        <div></div>
    </div>
</template>
<script>
    import BurgerMenu from './burger-menu.vue'
    export default {
        name: 'NavBar',
        data() {
            return {
                active:true,
            }
        },
        components: {
            BurgerMenu,
        },
        mounted(){
            this.active = true;
        }
    }
</script>

<style lang="less" scoped>
  @import './navbar.less';
</style>


