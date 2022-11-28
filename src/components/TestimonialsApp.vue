<script>
import Cta_Btn from './Cta_Btn.vue'

export default {
    name: 'TestimonialsApp',
    components:{
      Cta_Btn,
    },
    data(){
      return{
        call: 'READ MORE TESTIMONIALS',
      }
    }
}
</script>

<template>
  <section>
  <div class="testimonials">
    <div class="tocenter">
          <div class="ac-container">
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
              <Cta_Btn v-html="call" />
            </div>
          </div>  
        </div>
      </section>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

.testimonials{
  background-image: url(../assets/img/avada-movers-testimonial-background.jpg);
  background-size: cover;
  background-position: center;
  font-size: 8px;
  height: 508px;
  .tocenter{
    height: 100%;
    .ac-container{
      height: 100%;
    }
  }
}

</style>