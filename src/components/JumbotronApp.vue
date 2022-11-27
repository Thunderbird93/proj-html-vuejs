<script>
import MenuApp from './MenuApp.vue'
import pagine from '../data/menu'

export default {
    name: 'JumbotronApp',
    props:{
    },
    components:{
        MenuApp
    },
    data(){
        return{
            pagine
        }
    }
}
</script>

<template>
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
                        <MenuApp :menu="pagine" />
                    </ul>
                    <div class="cta-btn">

                    </div>
                </nav>
            </div>
            <!-- /Top Jumbotron -->

            <!-- Bottom Jumbotron -->
            <div class="j-bottom">
              <div>
                <h6>MOVING WITHOUT THE HASSLE</h6>
                <h2>WE MAKE T SIMPLE</h2>
                <h6>PROFESSIONAL SERVICE WITH QUALITY AND CUSTOMER SATISFACTION</h6>
              </div>
            </div>
            <!-- /Bottom Jumbotron -->
        </div>
    </div>
    <!-- /Jumbotron -->
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
        }
    }
    .j-bottom{
        @include center;
        @include debug;
    }
}

</style>