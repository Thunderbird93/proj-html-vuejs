<script>
export default {
    name: 'CtaApp'
}
</script>

<template>
<div class="cta">
    <span>
      <i class="fa-regular fa-paper-plane"></i>
      <h5>GET A FREE QUOTE ONLINE NOW!</h5>
    </span>
</div>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;
.cta{
    background-color: $md-denim;
    @include center;
    height: 71px;
    span{
      display: flex;
      color: $cc-white;
      h5{
        margin-left: 5px;
      }
    }
  }
</style>