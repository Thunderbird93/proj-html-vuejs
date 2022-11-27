<script>
import MenuApp from './MenuApp.vue'
import Cta_Btn from './Cta_Btn.vue'
import pagine from '../data/menu'

export default {
    name: 'JumbotronApp',
    props:{
    },
    components:{
        MenuApp,
        Cta_Btn
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
                        <img src="../assets/img/avada-movers-retinalogo.png" alt="logo">
                    </a>
                </div>
                <navbar>
                    <ul>
                        <MenuApp :menu="pagine" />
                        <Cta_Btn />
                    </ul>
                </navbar>
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
    height: 396px;
    .j-top{
        font-size: 9px;
        display: flex;
        justify-content: space-between;
        height: 50px;
        margin-top: 10px;
        .navbar{
            display: flex;
        }
        .j-bottom{
            @include center;
            @include debug;
        }
        .logo{
            height: 100%;
                a{
                    height: 100%;
                    img{
                        height: 35px;
                    }
                }
        }
        ul{
            @include center;
            font-weight: 900;
        }
    }
}

</style>