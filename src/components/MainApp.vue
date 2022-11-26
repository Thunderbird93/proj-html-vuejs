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
        <div class="ac-container">
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
      </div>
      <!-- 3-Cards -->
      <div class="ac-container">
        <div class="tre-carte d-flex">
          <!-- 1ª carta -->
          <div class="ac-container">
            <div class="card">
              <img class="card-img-top" src="../assets/img/avada-movers-serviceonephoto-final.jpg" alt="Card image cap">
              <div class="card-body">
                <h5 class="card-title">Card title</h5>
                <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                <a href="#" class="btn btn-primary">Go somewhere</a>
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
                <a href="#" class="btn btn-primary">Go somewhere</a>
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
                <a href="#" class="btn btn-primary">Go somewhere</a>
              </div>
            </div>
          </div>
        </div>
      </div>  
      <!-- /3-Cards -->
      <!-- Move with Ease -->
      <div class="ease">
        <div class="ac-container">
          <div class="cta-card">
            <div class="card text-center" style="width: 18rem;">
              <div class="card-body">
                <h5 class="card-title">Special title treatment</h5>
                <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                <a href="#" class="btn btn-primary">Go somewhere</a>
              </div>
            </div>
          </div>
        </div>
      </div>
      <!-- /Move with Ease -->
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
  .ease{
    height: 400px;
    background-image: url(../assets/img/avada-movers-servicetwophoto-final.jpg);
    background-size: cover;
    background-position: center;
  }
}


</style>

