<script>
import Cta_Btn from './Cta_Btn.vue'
import testimonianze from '../data/testimonials'

export default {
    name: 'TestimonialsApp',
    components:{
      Cta_Btn,
    },
    data(){
      return{
        call: 'READ MORE TESTIMONIALS',
        testimonianze,
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
                <div v-for="(testimonianza, index) in testimonianze" :key="index"  class="col-md-4 mb-5 mb-md-0">
                  <div class="d-flex justify-content-center mb-4">
                    <img :src="[testimonianza.img]"
                      class="rounded-circle shadow-1-strong" height="150" />
                  </div>
                  <h5 class="mb-3">{{testimonianza.nome}}</h5>
                  <p class="px-xl-3">
                    {{testimonianza.voce}}
                  </p>
                </div>
               </div>
               <div class="temp">
                <Cta_Btn v-html="call" />
               </div>
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
      img{
        width: 100px;
        height: 100px;
      }
      .temp{
        display: flex;
        justify-content: center;
        }
    }
  }
}

</style>