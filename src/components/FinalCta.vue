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
      <h2>Request A Free Quote</h2>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Corporis voluptatibus ipsum est adipisci sapiente possimus pariatur aperiam iure ducimus quisquam nam quidem, reprehenderit iste nobis dolore maiores voluptas ullam sit.</p>
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
    text-align: center;
    @include center;
  }
}
</style>