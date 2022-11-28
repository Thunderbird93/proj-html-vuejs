<script>
import MenuApp from './MenuApp.vue'
import PostsApp from './PostsApp.vue'
import pagine from '../data/menu'
import posts from '../data/posts'
import immagini from '../data/logo'
export default {
    name: 'FooterTop',
    components:{
      MenuApp,
      PostsApp,
    },
    props:{
      posts: Object
    },
    data(){
      return{
        pagine,
        posts,
        immagini
      }
    }
}
</script>

<template>
    <div class="mid-line"></div>
    <div class="footer-top">
      <div class="ac-container">
        <div class="about">
          <h6>ABOUT</h6>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga dolores aspernatur maiores accusamus eaque amet possimus odit vel quaerat magni? Facere esse eum consectetur quo inventore repellendus! Rerum, ipsa non?</p>
          <div class="logo">
            <a v-for="(immagine, index) in immagini" :key="index" href="#">
              <img :src="immagine.path" :alt="immagine.nome">
            </a>
          </div>
        </div>
        <div class="movers">
          <h6>Movers</h6>
          <MenuApp :menu="pagine" />
        </div>
        <div class="posts">
          <h6>RECENT POSTS</h6>
          <PostsApp :posts="posts" />
        </div>
      </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;
  .mid-line{
    height: 8px;
    background-color: $cc-lima;
  }
  .footer-top{
    height: 225px;
    .ac-container{
      display: flex;
          .about{
            width: 30%;
            margin-right: 100px;
            .logo{
            }
          }
          .movers{
            margin-right: 100px;
          }
    }  
  }
</style>