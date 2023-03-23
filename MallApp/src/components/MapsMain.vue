<template>
  <div class="hero">
    <div class="hero__search">
      <FilterMap />
    </div>
    <div class="hero__maps">
      <img
        id="floorMap"
        src="../assets/images/first_floor_app.webp"
        alt="image of first floor"
      />
    </div>
    <div class="hero__selectFloors">
      <button @click="changeFloor('/src/assets/images/basement_app.webp')">
        <p>Basement</p>
      </button>
      <button
        class="hero__activeMaps"
        @click="changeFloor('/src/assets/images/ground_floor_app.webp')"
      >
        <p>Ground floor</p>
      </button>
      <button @click="changeFloor('/src/assets/images/first_floor_app.webp')">
        <p>First floor</p>
      </button>
    </div>
  </div>
</template>

<script setup>
import FilterMap from "./FilterMap.vue";

function changeFloor(imgUrl) {
  let img = document.querySelector("#floorMap");
  img.setAttribute("src", imgUrl);
}
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
    font-size: 14px;
    color: #888;
    font-weight: 600;
    cursor: pointer;
    text-align: center;
  }
  span {
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    font-size: 15px;
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
  &__selectFloors {
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: end;
  }
  &__selectFloors button {
    padding: 4px 10px;
    width: 164px;
    border-radius: 4px;
    background-color: transparent;
    border: none;
    transition: transform 0.2s;
  }
  &__activeMaps p {
    font-size: 15px;
    color: $white;
    background-color: $purple;
    border-radius: 4px;
    padding: 8px 10px;
  }
}
/* mobile responsive */
@media (max-width: $mobile) {
  header {
    margin-bottom: 10%;
  }
  .hero {
    flex-direction: column;
    &__search {
      justify-content: center;
      margin-bottom: 10%;
    }
    img {
      width: 100%;
    }
    p {
      font-size: 13px;
    }
    span {
      font-size: 14px;
    }
    &__selectFloors {
      margin-top: 10%;
      margin-bottom: 10%;
      align-items: center;
    }
    &__selectFloors button {
      width: 144px;
      padding-left: 6px;
      padding-right: 6px;
    }
    &__activeMaps p {
      font-size: 14px;
    }
  }
}
</style>
