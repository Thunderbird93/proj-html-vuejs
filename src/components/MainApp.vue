<script>
import CtaApp from './CtaApp.vue'
import MiddleJumbotron from './MiddleJumbotron.vue'
import TreCarteApp from './TreCarteApp.vue'
import MoveEase from './MoveEase.vue'
import TestimonialsApp from './TestimonialsApp.vue'
import FinalCta from './FinalCta.vue'

export default {
    name: 'MainApp',
    components:{
      CtaApp,
      MiddleJumbotron,
      TreCarteApp,
      MoveEase,
      TestimonialsApp,
      FinalCta
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
      <FinalCta />
    </main>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

main{
}
</style>

