<template>
  <nav>
    <router-link :to="{name:'home'}"> Главная </router-link>
    <router-link :to="{name:'katalog'}"> Каталог </router-link>
    <router-link :to="{name:'about'}"> О нас </router-link>
  </nav>
  <router-view/>
  <FooterComponent></FooterComponent>
</template>
<script>
import FooterComponent from './components/FooterComponent.vue';

export default {
  name: 'App',
  components:{FooterComponent}
}
</script>



<style>
body {
  margin: 0px;
  }

nav {
  background-color: black;
  width: 100%;
  height: 50px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  gap: 20px;
}

nav a {

  color: silver;
  font-size: 35px;
  text-decoration: none;
  font-family: 'Times New Roman', Times, serif;
}

nav a:hover {
  color: white;
}
</style>

