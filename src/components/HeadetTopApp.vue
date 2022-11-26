<script>
export default {
    name: HeaderTopApp,
    props:{
        social: Object,
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
        </div>
    </div>
</template>

<style>

</style>