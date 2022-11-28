<script>
import Cta_Btn from './Cta_Btn.vue'
export default {
    name: 'MoveEase',
    components:{
      Cta_Btn,
    },
    data(){
      return{
        call: 'GET A FREE QUOTE NOW',
      }
    }
}
</script>

<template>
  <div class="ease">
        <div class="ac-container">
          <div class="cta-card">
            <div class="card text-center" style="width: 18rem;">
              <div class="card-body carta">
                <h5 class="card-title">Move With Ease</h5>
                <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                <div class="temp">
                 <Cta_Btn v-html="call" />
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
  .ease{
    height: 400px;
    background-image: url(../assets/img/avada-movers-servicetwophoto-final.jpg);
    background-size: cover;
    background-position: center;
    display: flex;
    align-items: center;
    .cta-card{
      display: flex;
      justify-content: flex-end;
      .carta{
        color: $cc-white;
        background-color: $cc-lima;
        border: 5px solid $mc-hippie-green;
        .temp{
        display: flex;
        justify-content: center;
        }
      }
    }
  }
</style>