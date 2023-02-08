<script setup>
import PostAreaApp from './components/PostAreaApp.vue'
  import {
    RouterLink,
    RouterView
  } from 'vue-router'
</script>

<template>
  <header>
    <!-- <nav>
    <RouterLink to="/">Home</RouterLink>
    <RouterLink to="/contact">Contact</RouterLink>
  </nav> -->

    <div class="header__wrapper">
      <img src="../src/assets/images/logo_mall_app.png" height="" alt="logo of mall app">
      <h1>Welcome</h1>
    </div>
   
  </header>
 

  <RouterView />
  <PostAreaApp/>
</template>

<style lang="scss">
  header {
  max-width: 1140px;
  margin: 0 auto;
  position: relative;
  }
header::after {
  content: "";
  background-image: url('../assets/images/BG_map.webp');
  opacity: 0.1;
  background-position-x: center;
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: fixed;
  position: absolute;
  top: 0px;
  right: 0px;
  bottom: 0px;
  left: 0px;
}

.header__wrapper {
  
  display: flex;
  
  justify-content: space-around;
  align-items: center;
}

  .header__wrapper img {
    width: 176px;
    height: 109px;
  }
  .header__wrapper h1 {
    color: #FFFFFF;
    font-family: "Roboto", Sans-serif;
    font-size: 30px;
    font-weight: 600;
  } 

</style>