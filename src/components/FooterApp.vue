<script>
export default {
    name: 'FooterApp',
    data(){
      return{
      }
    }
}
</script>

<template>
  <footer>
    <div class="mid-line"></div>
    <!-- Footer Top -->
    <div class="footer-top">
      <div class="ac-container"></div>
    </div>
    <!-- /Footer Top -->
    <!-- Footer Bottom -->
    <div class="footer-bottom">
      <div class="ac-container"></div>
    </div>
    <!-- /Footer Bottom -->
  </footer>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

footer{
  .mid-line{
    height: 20px;
    background-color: $cc-lima;
  }
  .footer-top{
    height: 300px;
  }
  .footer-bottom{
    height: 200px;
    background-color: $cc-lima;
  }
}

</style>