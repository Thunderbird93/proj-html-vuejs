<script>
export default {
    name: 'Cta_Btn'
}
</script>

<template>
  <span></span>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

span{
  @include center;
  @include cta_btn;
  
}

</style>