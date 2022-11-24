<script>
export default {
    name: 'HeaderApp',
    props:{
        social: Array
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
        <div class="container">
            <div class="cta">
                <i class="fa-solid fa-phone-flip"></i>
                <span>Call us for a Free Quote: (numero verde)</span></div>
            <div class="social">
                <ul>
                    <li v-for="(icon, index) in social" :key="index">
                        <a :href="icon.path" target="_blank" rel="noopener noreferrer">
                            <p v-html="icon.img"></p>
                        </a>
                    </li>
                </ul>
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
    .container{
        color: $cc-white;
        display: flex;
        justify-content: space-between;
        align-items: center;
    } .social{
        ul{
            display: flex;
        }
    }
}

</style>