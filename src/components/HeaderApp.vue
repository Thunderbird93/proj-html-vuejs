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
                </nav>
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
    .j-top{
        display: flex;
        justify-content: space-between;
        li{
            a{
                color: black;
            }
        }
    }
}

</style>