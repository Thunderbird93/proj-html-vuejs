<script>
import CtaApp from './CtaApp.vue'
import MiddleJumbotron from './MiddleJumbotron.vue'
import TreCarteApp from './TreCarteApp.vue'
import MoveEase from './MoveEase.vue'
import TestimonialsApp from './TestimonialsApp.vue'

export default {
    name: 'MainApp',
    components:{
      CtaApp,
      MiddleJumbotron,
      TreCarteApp,
      MoveEase,
      TestimonialsApp
    }
}
</script>

<template>
    <main>
      <CtaApp />
      <MiddleJumbotron />
      <TreCarteApp /> 
      <MoveEase />
      <TestimonialsApp />
      <!-- /Testimonials-->
      <!-- final-CTA -->
      <div class="final-cta">
        <div class="ac-container">
          
        </div>
        <!-- /final-CTA -->
      </div>
    </main>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

main{
  .final-cta{
    background-image: url(../assets/img/avada-movers-request-quote-background.jpg);
    height: 300px;
  }
}

</style>

