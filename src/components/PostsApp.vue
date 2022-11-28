<script>
export default {
    name: 'PostsApp',
    props:{
        posts: Object
    }
}
</script>

<template>
  <li v-for="(post, index) in posts" :key="index">
    <a :href="post.path">{{post.nome}}</a>
  </li>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

li{
  margin: 5px 15px;
     a{
        color: black;
        font-weight: bolder;
        font-size: 8px;
    }
}
</style>