<script>
import FooterTop from './FooterTop.vue'
import FooterBottom from './FooterBottom.vue'

export default {
    name: 'FooterApp',
    components:{
      FooterTop,
      FooterBottom
    },
    data(){
      return{
      }
    }
}
</script>

<template>
  <footer>
    <FooterTop />
    <FooterBottom />
  </footer>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

footer{
}

</style>