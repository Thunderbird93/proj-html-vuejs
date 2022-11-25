<script>
export default {
    name: 'HeaderApp',
    props:{
        social: Array,
        menu: Array
    },
    data(){
        return{
        }
    }
}
</script>

<template>
  <header>
    <div class="header-top">
        <div class="ac-container">
            <div class="cta">
                <i class="fa-solid fa-phone-flip"></i>
                <span>Call us for a Free Quote: 1.800.555.6789</span></div>
            <div class="social">
                <ul>
                    <li v-for="(icon, index) in social" :key="index">
                        <a :href="icon.path" target="_blank" rel="noopener noreferrer">
                            <span v-html="icon.img"></span>
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
    <div class="ac-jumbotron">
        <div class="ac-container">
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
            <div class="j-bottom">
                <h6>MOVING WITHOUT THE HASSLE</h6>
                <h2>WE MAKE IT SIMPLE</h2>
                <h6>PROFESSIONAL SERVICE WITH QUALITY AND CUSTOMER SATISFACTION</h6>
            </div>
        </div>
    </div>
  </header>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

.header-top{
    background-color: $cc-lima;
    height: 50px;
    .ac-container{
        color: $cc-white;
        display: flex;
        justify-content: space-between;
        align-items: center;
    } .social{
        ul{
            display: flex;
            align-items: center;
            margin: 0;
        }
    }
}
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