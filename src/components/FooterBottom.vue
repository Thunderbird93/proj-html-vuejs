
<script>
export default {
    name: 'FooterBottom',
}
</script>

<template>
    <div class="footer-bottom">
      <div class="ac-container"></div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;
.footer-bottom{
    height: 200px;
    background-color: $cc-lima;
  }
</style>