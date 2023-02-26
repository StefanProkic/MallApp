<template>
  <div class="productsPost">
    <h3>Best offers</h3>
    <div class="productsPost__wrapper">
      <div class="productsPost__box">
        <h4>special offer</h4>
        <h2>sweater - zara</h2>
        <div class="productsPost__image">
          <img src="../assets/images/sweater_zara.webp" alt="" />
        </div>
      </div>
      <div class="productsPost__box">
        <h4>special offer</h4>
        <h2>sweater - zara</h2>
        <div class="productsPost__image">
          <img src="../assets/images/sweater_zara.webp" alt="" />
        </div>
      </div>
      <div class="productsPost__box">
        <h4>special offer</h4>
        <h2>sweater - zara</h2>
        <div class="productsPost__image">
          <img src="../assets/images/sweater_zara.webp" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.productsPost {
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
