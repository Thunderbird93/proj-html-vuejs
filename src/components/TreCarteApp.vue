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
  <div class="ac-container">
        <div class="tre-carte d-flex">
          <!-- 1ª carta -->
          <div class="ac-container">
            <div class="card">
              <img class="card-img-top" src="../assets/img/avada-movers-serviceonephoto-final.jpg" alt="Card image cap">
              <div class="card-body">
                <h5 class="card-title">Card title</h5>
                <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                <Cta_Btn />
              </div>
            </div>
          </div>
          <!-- 2ª carta -->
          <div class="ac-container">
            <div class="card">
              <img class="card-img-top" src="../assets/img/avada-movers-servicetwophoto-final.jpg" alt="Card image cap">
              <div class="card-body">
                <h5 class="card-title">Card title</h5>
                <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                <Cta_Btn />
              </div>
            </div>
          </div>
          <!-- 3ª carta -->
          <div class="ac-container">
            <div class="card">
              <img class="card-img-top" src="../assets/img/avada-movers-servicethreephoto-final.jpg" alt="Card image cap">
              <div class="card-body">
                <h5 class="card-title">Card title</h5>
                <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                <Cta_Btn />
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

.ac-container{
  height: 548px;
}

</style>