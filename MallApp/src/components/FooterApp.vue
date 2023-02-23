<template>
  <footer>
    <RouterLink to="/"
      ><img src="../assets/images/home.png" alt="Homepage icon"
    /></RouterLink>
    <RouterLink to="/contact"
      ><img src="../assets/images/map-pin.png" alt="Map pin icon"
    /></RouterLink>
  </footer>
</template>

<style lang="scss">
footer {
  display: flex;
  gap: 50px;
  justify-content: center;
  padding: 20px 0;
}
footer img {
  width: 50px;
}
</style>
<script setup>
import { RouterLink } from "vue-router";
</script>
