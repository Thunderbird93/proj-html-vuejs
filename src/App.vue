<script>
import HeaderApp from './components/HeaderApp.vue'
import MainApp from './components/MainApp.vue'
import FooterApp from './components/FooterApp.vue'

export default {
  name: 'App',
  components:{
    HeaderApp,
    MainApp,
    FooterApp
  }
}
</script>

<template>
  <HeaderApp />
  <MainApp />
  <FooterApp />
</template>

<style lang="scss" scoped>
@use './style/general.scss';
@use './style/partials/mixin' as *;
@use './style/partials/variables' as *;

</style>