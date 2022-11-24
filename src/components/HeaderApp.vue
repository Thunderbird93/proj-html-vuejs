<script>
export default {
    name: 'HeaderApp'
}
</script>

<template>
  <header>
    <div class="header-top">
        <div class="container">
            <div class="cta">Call us for a Free Quote: (numero verde)</div>
            <div class="social">le 4 icone social</div>
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