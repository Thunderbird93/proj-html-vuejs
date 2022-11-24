<script>
import HeaderApp from './components/HeaderApp.vue'
import MainApp from './components/MainApp.vue'
import FooterApp from './components/FooterApp.vue'
import isocial from './data/social'

export default {
  name: 'App',
  components:{
    HeaderApp,
    MainApp,
    FooterApp
  },
  data(){
    return{
      isocial,
    }
  }
}
</script>

<template>
  <HeaderApp :social="isocial" />
  <MainApp />
  <FooterApp />
</template>

<style lang="scss" scoped>
@use './style/general.scss';
@use './style/partials/mixin' as *;
@use './style/partials/variables' as *;

</style>