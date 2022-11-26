<script>
import SocialApp from './SocialApp.vue'

export default {
    name: 'HeaderTopApp',
    props:{
        social: Object,
    },
    components:{
        SocialApp
    }
}
</script>

<template>
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
            <SocialApp />
        </div>
    </div>
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
</style>