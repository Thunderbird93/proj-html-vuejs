<script>
import HeaderApp from './components/HeaderApp.vue';
import MainApp from './components/MainApp.vue';
import FooterApp from './components/FooterApp.vue';
import icons from './data/social';

export default {
  name: 'App',
  components:{
    HeaderApp,
    MainApp,
    FooterApp
  },
  data(){
    return{
      icons,
    }
  }
}
</script>

<template>
  <HeaderApp :social="icons"/>
  <MainApp />
  <FooterApp />
</template>

<style lang="scss" scoped>
@use './style/general.scss';
@use './style/partials/mixin' as *;
@use './style/partials/variables' as *;

</style>