
<script>
import SocialApp from './SocialApp.vue'
import icons from '../data/social'

export default {
    name: 'FooterBottom',
    components:{
      SocialApp,
    },
    data(){
      return{
        icons,
      }
    }
}
</script>

<template>
    <div class="footer-bottom">
      <div class="ac-container">
        <!--About-->
        <div class="about"></div>
        <!--Copyright-->
        <div class="copyright">
          <p>&copy Copyright 2012 - 2020</p>
          <p>|</p>
          <p>Avada Theme by ThemeFusion</p>
          <p>|</p>
          <p>Powered by WordPress</p>
        </div>
        <SocialApp :social="icons"/>
      </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;
.footer-bottom{
    height: 72px;
    background-color: $cc-lima;
    color: $cc-white;
    display: flex;
    flex-direction: column;
    justify-content: center;
    .copyright{
      display: flex;
      justify-content: center;
    }
  }
</style>