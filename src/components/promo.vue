<template>
  <div class="promo">
    <div class="promo__bg"></div>
    <div class="promo__quote">
      <div class="promo__quote-header">
        <img src="../assets/logopromo.svg" alt="logo" />
        <h1>Новая коллекция французских авторов</h1>
      </div>

      <span
        >Сложно сказать, почему акционеры крупнейших компаний призывают нас к
        новым свершениям, которые, в свою очередь, должны быть заблокированы в
        рамках своих собственных рациональных ограничений. <br />
        <p>
          Принимая во внимание показатели успешности, граница обучения кадров
          предопределяет высокую востребованность направлений прогрессивного
          развития.
        </p></span
      >
      <button>Ознакомиться</button>
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
  background-size: contain;
  z-index: 1;
  position: absolute;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  justify-items: center;
  position: absolute;
  background-size: cover;
  background: linear-gradient(
    to right,
    rgba(1, 1, 2, 0.75) 0%,
    rgba(13, 43, 67, 0.9) 45%,
    rgba(0, 0, 0, 0.1) 65%
  );
  filter: contrast(120%);
}
.promo__quote {
  margin-top: 50px;
  width: 45%;
  height: auto;
  position: absolute;
  white-space: pre-line;
  margin-left: 120px;
  z-index: 2;
  text-align: start;
  flex-direction: column;
  .promo__quote-header {
    margin-bottom: 15px;
    display: flex;
    align-items: center;
    img {
      width: 150px;
      height: 130px;
    }
    h1 {
      font-family: base-font;
      color: rgba(244, 246, 245, 1);
      font-weight: 500;
      font-size: 45px;
      margin-left: 35px;
    }
  }
  span {
    font-family: base-font;
    color: rgba(244, 246, 245, 1);
    font-weight: 500;
    font-size: 20px;
    p {
      margin-top: 25px;
    }
  }
  button {
    outline: none;
    background-color: rgba(238, 219, 109, 1);
    color: rgba(44, 45, 53, 1);
    border: none;
    font-family: base-font;
    font-weight: 500;
    font-size: 25px;
    padding: 20px, 60px, 20px, 60px;
    gap: 10px;
    margin-top: 70px;
    width: 200px;
    height: 60px;
    cursor: pointer;
  }
}
</style>