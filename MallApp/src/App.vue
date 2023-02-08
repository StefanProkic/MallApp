<script setup>
import PostAreaApp from "./components/PostAreaApp.vue";
import Map from "./components/MapApp.vue";
/*  import {
    RouterLink,
    RouterView
  } from 'vue-router' */
</script>

<template>
  <header>
    <!-- <nav>
    <RouterLink to="/">Home</RouterLink>
    <RouterLink to="/contact">Contact</RouterLink>
  </nav> -->

    <div class="header__wrapper">
      <img
        src="../src/assets/images/logo_mall_app.png"
        alt="logo of mall app"
      />
      <h1>Welcome</h1>
    </div>
  </header>
  <Map />

  <RouterView />
  <PostAreaApp />
</template>

<style lang="scss">
header {
  max-width: 1140px;
  margin: 0 auto;
  position: relative;

  .header__wrapper {
    display: flex;
    justify-content: space-around;
    align-items: center;

    img {
      width: 176px;
      height: 109px;
    }

    h1 {
      color: #ffffff;
      font-family: "Roboto", Sans-serif;
      font-size: 30px;
      font-weight: 600;
    }
  }
}
</style>
