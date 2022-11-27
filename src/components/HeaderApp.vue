<script>
import HeaderTopApp from './HeaderTopApp.vue'
import JumbotronApp from './JumbotronApp.vue' 

export default {
    name: 'HeaderApp',
    components:{
        HeaderTopApp,
        JumbotronApp
    },
    data(){
        return{
        }
    }
}
</script>

<template>
  <header>
    <!--Header Top-->
    <HeaderTopApp />
    <!--/Header Top-->

    <!-- Jumbotron -->
    <JumbotronApp />
    <!-- /Jumbotron -->
  </header>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;


</style>

