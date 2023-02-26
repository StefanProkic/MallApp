<template>
  <div class="storePost">
    <h3>Trending</h3>
    <div class="storePost__wrapper">
      <div class="storePost__box">
        <h4>clothing</h4>
        <h2>Nike</h2>
        <div class="storePost__image">
          <img src="../assets/images/nike.webp" alt="" />
        </div>
      </div>
      <div class="storePost__box">
        <h4>clothing</h4>
        <h2>Nike</h2>
        <div class="storePost__image">
          <img src="../assets/images/nike.webp" alt="" />
        </div>
      </div>
      <div class="storePost__box">
        <h4>clothing</h4>
        <h2>Nike</h2>
        <div class="storePost__image">
          <img src="../assets/images/nike.webp" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.storePost {
  padding-top: 40px;
  padding-bottom: 40px;
  height: 100%;
  width: 100%;

  &__wrapper {
    display: grid;
    grid-template-columns: repeat(3, 320px);
    grid-template-rows: 367px;
    gap: 90px;
    padding-top: 40px;
  }
  &__box {
    background: $purpleGradient;
    border-radius: 4px;
    padding: 20px;
  }
  &__box h4,
  h2 {
    margin-bottom: 12px;
  }
  &__image {
    overflow: hidden;
    display: flex;
    justify-content: center;
    border-radius: 4px;
    height: 242px;
  }
}
</style>
