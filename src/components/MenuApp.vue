<script>
export default {
    name: 'MenuApp',
    props:{
        menu: Object
    }
}
</script>

<template>
  <li v-for="(pagina, index) in menu" :key="index">
    <a :href="pagina.path">{{pagina.nome}}</a>
  </li>
</template>

<style lang="scss" scoped>
@use '../style/general.scss';
@use '../style/partials/mixin' as *;
@use '../style/partials/variables' as *;

li{
  margin: 5px;
     a{
        color: black;
        font-weight: bolder;
    }
}
</style>