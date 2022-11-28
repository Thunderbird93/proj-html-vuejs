
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
        <div class="copyright">
          <div>&copy Copyright 2012 - 2020</div>
          <div>|</div>
          <div>Avada Theme by ThemeFusion</div>
          <div>|</div>
          <div>Powered by WordPress</div>
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