<script>
import HeaderTopApp from './HeadetTopApp.vue'
import icons from '../data/social'

export default {
    name: 'HeaderApp',
    props:{
        menu: Object
    },
    components:{
        HeaderTopApp,
    },
    data(){
        return{
            icons
        }
    }
}
</script>

<template>
  <header>
    <!--Header Top-->
    <HeaderTopApp :social="icons"/>
    <!--/Header Top-->

    <!-- Jumbotron -->
    <div class="ac-jumbotron">
        <div class="ac-container">
            <!-- Top Jumbotron -->
            <div class="j-top">
                <div class="logo">
                    <a href="#">
                        <img src="../assets/img/avada-movers-logo.png" alt="logo">
                    </a>
                </div>
                <nav>
                    <ul>
                        <li v-for="(pagina, index) in menu" :key="index">
                            <a :href="pagina.path">{{pagina.nome}}</a>
                        </li>
                    </ul>
                    <div class="cta-btn">

                    </div>
                </nav>
            </div>
            <!-- /Top Jumbotron -->

            <!-- Bottom Jumbotron -->
            <div class="j-bottom">
                <h6>MOVING WITHOUT THE HASSLE</h6>
                <h2>WE MAKE IT SIMPLE</h2>
                <h6>PROFESSIONAL SERVICE WITH QUALITY AND CUSTOMER SATISFACTION</h6>
            </div>
            <!-- /Bottom Jumbotron -->
        </div>
    </div>
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