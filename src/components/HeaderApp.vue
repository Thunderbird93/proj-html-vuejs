<script>
import HeaderTopApp from './HeaderTopApp.vue'
import JumbotronApp from './JumbotronApp.vue' 
import pagine from '../data/menu'

export default {
    name: 'HeaderApp',
    components:{
        HeaderTopApp,
        JumbotronApp
    },
    data(){
        return{
            pagine
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
    <JumbotronApp :menu="pagine" />
    <!-- /Jumbotron -->
  </header>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

.ac-jumbotron{
    background-image: url(../assets/img/avada-movers-homeherobackground-final.jpg);
    background-size: cover;
    height: 500px;
    .j-top{
        display: flex;
        justify-content: space-between;
        ul{
            display: flex;
            li{
                a{
                    color: black;
                }
            }
        }
    }
}

</style>

