<template>
  <div class="singleStore">
    <h2>Special offer</h2>
    <div class="singleStore__productsWrapper">
      <div class="singleStore__productsBox">
        <h3>sweater - nike</h3>
        <h4>$ 69.99</h4>
        <img src="@/assets/images/sweater_zara.webp" alt="sweater" />
        <p>
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Debitis
          corrupti mollitia iusto dignissimos quod obcaecati.
        </p>
      </div>
      <div class="singleStore__productsBox">
        <h3>sweater - nike</h3>
        <h4>$ 69.99</h4>
        <img src="@/assets/images/sweater_zara.webp" alt="sweater" />
        <p>
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Debitis
          corrupti mollitia iusto dignissimos quod obcaecati.
        </p>
      </div>
      <div class="singleStore__productsBox">
        <h3>sweater - nike</h3>
        <h4>$ 69.99</h4>
        <img src="@/assets/images/sweater_zara.webp" alt="sweater" />
        <p>
          Lorem ipsum dolor, sit amet consectetur adipisicing elit. Debitis
          corrupti mollitia iusto dignissimos quod obcaecati.
        </p>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
h2 {
  padding-bottom: 40px;
  font-size: 48px;
}
h3 {
  background-color: $purple;
  padding: 32px 16px;
  font-weight: 200;
  font-size: 35px;
}
h4 {
  color: $black;
  margin-top: 15px;
  font-size: 56px;
  font-weight: 100;
  margin-bottom: 10px;
}

.singleStore {
  padding-top: 40px;
  padding-bottom: 40px;

  &__productsWrapper {
    display: grid;
    grid-template-columns: repeat(3, 363px);
    grid-template-rows: 635px;
    gap: 25.2px;
  }
  &__productsBox {
    background: $white;
    text-align: center;
    border-radius: 4px;

    img {
      width: 296px;
    }
    p {
      margin-left: 10px;
      margin-right: 10px;
      margin-top: 15px;
    }
  }
}
</style>
