<script>
import CtaApp from './CtaApp.vue'
import MiddleJumbotron from './MiddleJumbotron.vue'
import TreCarteApp from './TreCarteApp.vue'
import MoveEase from './MoveEase.vue'

export default {
    name: 'MainApp',
    components:{
      CtaApp,
      MiddleJumbotron,
      TreCarteApp,
      MoveEase
    }
}
</script>

<template>
    <main>
      <CtaApp />
      <MiddleJumbotron />
      <TreCarteApp /> 
      <MoveEase />
      <!-- Testimonials -->
      <div class="testimonials">
        <div class="ac-container">
          <section>
              <div class="row d-flex justify-content-center">
                <div class="col-md-10 col-xl-8 text-center">
                  <h3 class="mb-4">Testimonials</h3>
                  <p class="mb-4 pb-2 mb-md-5 pb-md-0">
                    Lorem ipsum dolor sit amet, consectetur adipisicing elit. Fugit, error amet
                    numquam iure provident voluptate esse quasi, veritatis totam voluptas nostrum
                    quisquam eum porro a pariatur veniam.
                  </p>
                </div>
              </div>

            <div class="row text-center">
              <!-- Prima Carta -->
              <div class="col-md-4 mb-5 mb-md-0">
                <div class="d-flex justify-content-center mb-4">
                  <img src="../assets/img/avada-movers-johndoe-final-200x200.jpg"
                    class="rounded-circle shadow-1-strong" height="150" />
                </div>
                <h5 class="mb-3">John Doe</h5>
                <p class="px-xl-3">
                  Lorem ipsum dolor sit amet, consectetur
                  adipisicing elit. Quod eos id officiis hic tenetur quae quaerat ad velit ab hic
                  tenetur.
                </p>
              </div>
              <!-- Seconda Carta -->
              <div class="col-md-4 mb-5 mb-md-0">
                <div class="d-flex justify-content-center mb-4">
                  <img src="../assets/img/avada-movers-janedoe-final-200x200.jpg"
                    class="rounded-circle shadow-1-strong" width="150" height="150" />
                </div>
                <h5 class="mb-3">Jane Doe</h5>
                <p class="px-xl-3">
                  Ut enim ad minima veniam, quis nostrum
                  exercitationem ullam corporis suscipit laboriosam, nisi ut aliquid commodi.
                </p>
              </div>
              <!-- Terza Carta -->
              <div class="col-md-4 mb-0">
                <div class="d-flex justify-content-center mb-4">
                  <img src="../assets/img/avada-movers-johnsmith-final-200x200.jpg"
                    class="rounded-circle shadow-1-strong" width="150" height="150" />
                </div>
                <h5 class="mb-3">John Smith</h5>
                <p class="px-xl-3">
                  At vero eos et accusamus et iusto odio
                  dignissimos ducimus qui blanditiis praesentium voluptatum deleniti atque corrupti.
                </p>
              </div>
            </div>
          </section>
        </div>
      </div>
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

