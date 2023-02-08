
<template>
  <main>
    <div class="hero">
      <img src="../assets/images/first_floor_app.webp" alt="image of first floor">
    </div>
  </main>
</template>

<script setup>

</script>

<style lang="scss">
.hero {
  display: flex;
  justify-content: center;
  
 
  width: 100%;
}
.hero img {
  position: relative;
  
}
.hero::before {
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
</style>
