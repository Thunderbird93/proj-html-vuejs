<script>
import Cta_Btn from './Cta_Btn.vue'

export default {
    name: 'FinalCta',
    components:{
      Cta_Btn,
    }
}
</script>

<template>
    <div class="final-cta">
    <div class="ac-container">
      <Cta_Btn />
    </div>
  </div>
</template>


<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

main{
  .final-cta{
    background-image: url(../assets/img/avada-movers-request-quote-background.jpg);
    height: 268px;
  }
}
</style>