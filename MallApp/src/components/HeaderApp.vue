<template>
  <header>
    <div class="header__wrapper">
      <a href="/" title="Home Page">
        <img src="../assets/images/logo_mall_app.png" alt="logo of mall app" />
      </a>
      <h1>Welcome</h1>
    </div>
  </header>
  <!-- <Map /> -->
  <RouterView />
  <!-- <PostAreaApp /> -->
</template>
<style lang="scss">
header {
  max-width: 1140px;
  margin: 0 auto;
  position: relative;
  margin-bottom: 100px;

  .header__wrapper {
    padding-top: 10px;
    display: flex;
    justify-content: space-around;
    align-items: center;

    img {
      width: 176px;
      height: 109px;
    }

    h1 {
      color: #ffffff;
      font-size: 30px;
      font-weight: 600;
      text-transform: uppercase;
    }
  }
}
</style>
