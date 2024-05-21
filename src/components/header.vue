<template>
  <div class="header">
    <div class="contaner">
      <img alt="logo" src="../assets/logo.png" />
      <span>Ink. House</span>
    </div>
    <div class="nav">
      <button>Репродукции</button>
      <button>Новинки</button>
      <button>О нас</button>
      <button class="cart">
        <img alt="cart" src="../assets/Frame.svg" />
      </button>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "headerComponent",
});
</script>

<style scoped lang="scss">

.header {
  width: 1440px;
  height: 100px;
  background-color: #e1ede6;
  .contaner {
    margin-left: 165px;
    gap: 8px;
    display: flex;
    align-items: center;
    img {
      height: 45px;
      width: 45px;
    }
    span {
      font-family: base-font;
      color: #598d66;
      font-size: 20px;
      font-weight: 500;
    }
  }
}
@media (min-width: 1912px) {
  .header {
    width: 1920px;
    height: 100px;
    background-color: #e1ede6;
    display: flex;
    align-items: center;

    .contaner {
      width: auto;
      height: auto;
      margin-left: 180px;
      gap: 12px;
      img {
        height: 50px;
        width: 50px;
      }
      span {
        font-family: base-font;
        color: #598d66;
        font-size: 25px;
        font-weight: 500;
      }
    }
    .nav {
      display: flex;
      justify-content: end;
      gap: 30px;
      margin-left: auto;
      margin-right: 200px;
      button {
        outline: none;
        border: 0;
        background-color: inherit;
        font-family: base-font;
        font-size: 25px;
        color: #2c2d35;
        font-weight: 500;
        cursor: pointer;
        img {
          height: 25px;
          width: 25px;
        }
      }
      .cart {
        font-size: 0rem;
      }
    }
  }
}
</style>