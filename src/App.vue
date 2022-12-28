
<template>

  <div>
    <div class="site-name icon home">
      <img src="../public/image/drevo.png" class="logo" alt="Logo">
      <h1>
        Yggdrasil
      </h1>
    </div>
    <div class="avatar-block">
      <!-- <div class="avatar-block-fly">
        <img class="avatar" src="#">
      </div> -->
    </div>
  </div>


  <nav class="main-menu">
    <router-link to="/">Главная</router-link> |
    <router-link to="/catalog">Каталог</router-link> |
    <router-link to="/paymentanddelivery">Оплата и доставка</router-link> |
    <router-link to="/registration">Регистрация</router-link> |
    <router-link to="/about"> О нас</router-link>
  </nav>
  <div class="searh">
    <searh-top />
  </div>

  <div class="main-content">
    <div class="left-nenu">
      <menu-left />
    </div>
    <div class="content">
      <router-view />
    </div>
  </div>

  <footer>
      <img src="../public/image/drevo.png" class="logo logo-footer" alt="Logo">
      <h2>
        2022&nbsp;Volha Yaustratava&nbsp;
      </h2>
  </footer>
</template>
<script setup>
import MenuLeft from './components/template/MenuLeft.vue';
import SearhTop from './components/template/SearhTop.vue';
</script>


<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
