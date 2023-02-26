<template>
  <div class="hero hero--desktop">
    <div class="hero__search">
      <FilterMap />
    </div>
    <div class="hero__maps">
      <img
        src="../assets/images/first_floor_app.webp"
        alt="image of first floor"
      />
    </div>
    <div class="hero__selectMaps">
      <button><p>Basement</p></button>
      <button class="hero__activeMaps"><p>Ground floor</p></button>
      <button><p>First floor</p></button>
    </div>
  </div>
</template>

<script setup>
import FilterMap from "./FilterMap.vue";
</script>

<style lang="scss">
.hero {
  display: flex;
  justify-content: center;
  width: 100%;

  &__search {
    width: 100%;
    display: inline-flex;
  }
  p {
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    font-size: 12px;
    color: #888;
    font-weight: 600;
    cursor: pointer;
    text-align: center;
  }
  span {
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    font-size: 14px;
    color: #888;
    font-weight: 600;
    cursor: pointer;
    text-align: center;
  }

  &__maps {
    width: 100%;
    text-align: center;
  }

  img {
    margin: 0 auto;
  }
  &__selectMaps {
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: end;
  }
  &__selectMaps button {
    padding: 4px 10px;
    width: 134px;
    border-radius: 4px;
    background-color: transparent;
    border: none;
    transition: transform 0.2s;
  }
  &__activeMaps p {
    font-size: 13px;
    color: $white;
    background-color: $purple;
    border-radius: 4px;
    padding: 8px 10px;
  }
}
</style>
