<template>
  <div class="singleStore">
    <div class="singleStore__txt">
      <h1>Nike</h1>
      <p>
        Lorem ipsum dolor sit amet consectetur, adipisicing elit. Possimus
        voluptate repellat odit aliquam nisi veniam consectetur, doloremque
        molestias ducimus ab perferendis vitae similique, incidunt ratione
        dignissimos.<br /><br />
        veritatis ullam expedita, quisquam tempore totam? Libero id labore eos
        optio veniam officiis recusandae architecto ex hic, possimus nam error
        saepe eaque minus quis dolorem voluptate perferendis deserunt facere.
        Dicta ad quod sapiente nesciunt accusamus, eos inventore animi soluta,
        iste magnam nostrum, dolor ex!
      </p>
      <div class="singleStore__legend">
        <img src="@/assets/images/building.webp" alt="building" />
        <h2>first floor</h2>
      </div>
    </div>
    <div class="singleStore__info">
      <div class="singleStore__infoBox">
        <img src="../assets/images/time.webp" alt="clock" />
        <h3>working hours</h3>
        <span
          >Mon – Fri 10.00 – 22.00<br />
          Sat – Sun 10.00 – 22.00</span
        >
      </div>
      <div class="singleStore__infoBox">
        <img src="../assets/images/email.webp" alt="clock" />
        <h3>email</h3>
        <a href="mailto:nike@gmail.com"><span>nike@gmail.com</span></a>
      </div>
      <div class="singleStore__infoBox">
        <img src="../assets/images/web.webp" alt="clock" />
        <h3>web</h3>
        <a href="https://www.nike.com/" target="_blank"
          ><span>https://nike.com</span></a
        >
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.singleStore {
  display: flex;
  &__txt {
    width: 792px;
    border-left: 1px solid $white;
    padding: 20px;
  }
  h1 {
    font-size: 48px;
    margin-bottom: 20px;
  }
  p {
    margin-left: 20px;
    margin-right: 20px;
    margin-bottom: 80px;
    font-size: 16px;
    color: $white;
    line-height: 1.7em;
  }
  &__legend {
    text-align: center;
  }
  &__info {
    width: 348px;

    display: grid;
    grid-template-rows: repeat(3, 149px);
    grid-template-columns: 308px;
    gap: 15px;
    padding-left: 40px;
  }
  &__infoBox {
    background-color: $white;
    padding: 16px;
    border-radius: 4px;
    img {
      width: 40px;
    }
    h3 {
      color: $black;
    }
    span {
      color: $black;
      margin-top: 5px;
    }
    a {
      text-decoration: none;
      color: $black;
    }
  }
}
</style>
