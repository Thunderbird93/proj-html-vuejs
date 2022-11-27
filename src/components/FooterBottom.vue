
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
        <SocialApp :social="icons"/>
      </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;
.footer-bottom{
    height: 200px;
    background-color: $cc-lima;
  }
</style>