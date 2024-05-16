<template>
  <div class="promo">
    <div class="promo__bg"></div>
    <div class="promo__quote">
      <img src="../assets/logopromo.svg" alt="logo" />
      <h1>Новая коллекция французских авторов</h1>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "promoComponent",
});
</script>

<style lang="scss" scoped>
.promo {
  height: 574px;
  width: 1440px;
  background-image: url("../assets/promobg.png");
  background-size: contain;
  margin: auto;
  position: relative;
}
.promo__bg {
  height: 100%;
  width: 50%;
  mix-blend-mode: multiply;
  mix-blend-mode: soft-light;
  background-color: rgba(13, 43, 67, 0.8);
  background-size: contain;
  z-index: 1;
  position: absolute;
}
.promo__quote {
  width: 50%;
  height: 100%;
  display: flex;
  justify-content: end;
  margin-left: auto;
  z-index: 3;
  position: absolute;
  border: 1px solid rgb(0, 0, 0);
  padding: 50px 0px 0px 0px;
  text-wrap: wrap;

  img {
    width: 80px;
    height: 80px;
  }
}
</style>