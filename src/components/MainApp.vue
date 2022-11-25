<script>
export default {
    name: 'MainApp'
}
</script>

<template>
    <main>
      <div class="cta">
        <span>
          <i class="fa-regular fa-paper-plane"></i>
          <h5>GET A FREE QUOTE ONLINE NOW!</h5>
        </span>
      </div>
    </main>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

main{
  .cta{
    background-color: $md-denim;
    //debug
    height: 100px;
    span{
      display: flex;
    }
  }
}


</style>

