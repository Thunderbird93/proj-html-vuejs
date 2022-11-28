<script>
import Cta_Btn from './Cta_Btn.vue'

export default {
    name: 'TreCarteApp',
    components:{
      Cta_Btn,
    }
}
</script>

<template>
  <div class="ac-container-nh">
    <div class="tocenter">
            <div>
              <div class="testo">
                <p>WE ARE PROFESSIONAL</p>
                <h2>Full-Service Solution</h2>
              </div>
              <div class="tre-carte d-flex">
                <!-- 1ª carta -->
                <div class="a-container">
                  <div class="card carta">
                    <img class="card-img-top" src="../assets/img/avada-movers-serviceonephoto-final.jpg" alt="Card image cap">
                    <div class="card-body">
                      <h5 class="card-title">Two Man Teams</h5>
                      <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                      <Cta_Btn />
                    </div>
                  </div>
                </div>
                <!-- 2ª carta -->
                <div class="a-container">
                  <div class="card carta">
                    <img class="card-img-top" src="../assets/img/avada-movers-servicetwophoto-final.jpg" alt="Card image cap">
                    <div class="card-body">
                      <h5 class="card-title">We Do All The Lifting</h5>
                      <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                      <Cta_Btn />
                    </div>
                  </div>
                </div>
                <!-- 3ª carta -->
                <div class="a-container">
                  <div class="card carta">
                    <img class="card-img-top"  src="../assets/img/avada-movers-servicethreephoto-final.jpg" alt="Card image cap">
                    <div class="card-body">
                      <h5 class="card-title">Coast To Coast</h5>
                      <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                      <Cta_Btn />
                    </div>
                  </div>
                </div>
              </div>
            </div> 
          </div>   
      </div>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

.ac-container-nh{
  height: 548px;
  .tocenter{
    @include center;
    height: 100%;
    margin-top: 0px;
    .tre-carte{
      height: 340px;
          .testo{
            text-align: center;
          }
          .carta{
            border: 10px solid $mc-mercury;
            height: 100%;
            border-radius: 0;
            display: flex;
            margin: 0 15px;
            h5{
              font-size: 16px;
              text-align: center;
              font-weight: bolder;
              color: $cc-denim;
            }
            img{
              border-radius: 0;
              border-bottom: 10px solid $mc-mercury;
            }
        }
      }   
  }  
}

</style>