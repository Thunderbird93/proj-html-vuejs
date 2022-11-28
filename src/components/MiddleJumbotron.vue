<script>
import Cta_Btn from './Cta_Btn.vue'

export default {
    name: 'MiddleJumbotron',
    components:{
      Cta_Btn,
    }

}
</script>

<template>
  <div class="main-jumbotorn">
        <div class="ac-container">
          <div class="jumbotronn">
            <p>HEADACHE FREE</p>
            <h2>Award Winning</h2>
            <h2>Moving Company</h2>
            <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Dolore tenetur quia quas veritatis ullam illum voluptatem ad eligendi repellendus facilis sunt quisquam at, error reprehenderit iusto accusamus atque non alias illo, dolores laboriosam consequatur?</p>
            <Cta_Btn />
          </div>
        </div>  
      </div>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;
    .main-jumbotorn{
    background-color: $mc-mercury;
    height: 335px;
    .ac-container{
      @include center;
      .jumbotronn{
        text-align: center;
        font-size: 8px;
        width: 50%;
        margin: 0 auto;
        h2{
          font-size: 16px;
          color: $cc-lima;
          font-weight: bolder;
        }
      }
    }  
  }
</style>