<script>
import SocialApp from './SocialApp.vue'
import icons from '../data/social'

export default {
    name: 'HeaderTopApp',
    components:{
        SocialApp,
    },
    data(){
        return{
            icons,
            assistenza: '1.800.555.6789',
        }
    }
}
</script>

<template>
    <div class="header-top">
        <div class="ac-container">
            <!-- CTA -->
            <div class="cta">
                <i class="fa-solid fa-phone-flip"></i>
                <span>
                    Call us for a Free Quote: <a href="tel:+{{assistenza}}">{{assistenza}}</a>
                </span>
            </div>
            <!-- /CTA -->

            <!-- Componente -->
            <SocialApp :social="icons" /> 
            <!-- /Componente -->
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;
.header-top{
    background-color: $cc-lima;
    height: 30px;
    font-size: 10px;
    .ac-container{
        color: $cc-white;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
}
</style>