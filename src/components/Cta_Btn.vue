<script>
export default {
    name: 'Cta_Btn'
}
</script>

<template>
  <span>FREE QUOTE</span>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

span{
    @include cta_btn;
    @include center;
}

</style>