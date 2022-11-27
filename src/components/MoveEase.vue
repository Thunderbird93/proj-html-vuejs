<script>
export default {
    name: 'MoveEase',
}
</script>

<template>
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
  }
</style>