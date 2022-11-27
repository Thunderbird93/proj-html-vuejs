<script>
export default {
    name: 'FooterTop',
}
</script>

<template>
    <div class="mid-line"></div>
    <div class="footer-top">
      <div class="ac-container"></div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;
  .mid-line{
    height: 20px;
    background-color: $cc-lima;
  }
  .footer-top{
    height: 300px;
  }
</style>