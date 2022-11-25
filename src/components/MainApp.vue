<script>
export default {
    name: 'MainApp'
}
</script>

<template>
    <main>
      <!-- CTA -->
      <div class="cta">
        <span>
          <i class="fa-regular fa-paper-plane"></i>
          <h5>GET A FREE QUOTE ONLINE NOW!</h5>
        </span>
      </div>
      <!-- Jumbotron (Main) -->
      <div class="main-jumbotorn">
        <div class="jumbotron">
          <h6>HEADACHE FREE</h6>
          <h2 class="display-4">Award Winning</h2>
          <h2 class="display-4">Moving Company</h2>
          <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Dolore tenetur quia quas veritatis ullam illum voluptatem ad eligendi repellendus facilis sunt quisquam at, error reprehenderit iusto accusamus atque non alias illo, dolores laboriosam consequatur?</p>
          <p class="lead">
            <a class="btn btn-primary btn-lg" href="#" role="button">READ OUR TESTIMONIALS</a>
        </p>
</div>
      </div>
    </main>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

main{
  .cta{
    background-color: $md-denim;
    //debug
    height: 100px;
    span{
      display: flex;
    }
  }
  .main-jumbotorn{
    background-color: $mc-mercury;
  }
}


</style>

