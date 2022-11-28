<script>
import { objectToString } from '@vue/shared';

export default {
    name: 'SocialApp',
    props:{
        social: Object,
    },
    data(){
        return{

        }
    }
}
</script>

<template>
  <div class="social">
        <ul>
            <li v-for="(icon, index) in social" :key="index">
                <a :href="icon.path" target="_blank" rel="noopener noreferrer">
                    <span v-html="icon.img"></span>
                </a>
            </li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;
.social{
        ul{
            display: flex;
            align-items: center;
            margin: 0;
        } li {
            margin: 0 5px;
        }
        display: flex;
        justify-content: center;
    }
</style>