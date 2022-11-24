<script>
export default {
    name: 'HeaderApp'
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
                <i class="fa-brands fa-facebook-f"></i>
                <i class="fa-brands fa-twitter"></i>
                <i class="fa-brands fa-instagram"></i>
                <i class="fa-brands fa-youtube"></i>
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
    }
}

</style>