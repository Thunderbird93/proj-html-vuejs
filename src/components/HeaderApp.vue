<script>
export default {
    name: 'HeaderApp'
}
</script>

<template>
  <header>
    <div class="header-top">
        <div class="container">

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
}

</style>