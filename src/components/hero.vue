<template>
  <div class="hero">
    <div class="layer">
      <img alt="layer" src="../assets/Layer.png" />
    </div>
    <div class="frame">
      <h1>Реплики картин от <span>Ink. House </span></h1>
     <h2>Высокое качество отрисовки на плотной бумаге или льняном холсте. Редкие произведения, доступные цены.</h2>
     <button>Продукция</button>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "heroComponent",
});
</script>

<style scoped lang="scss">
.hero {
  height: 622px;
  display: flex;
  gap: 25px;
  align-items: center;
  .layer {
    width: 50%;
    display: flex;
    justify-content: end;
  }
  .frame {
    align-items: center;
    width: 540px ;
    height: auto;

    h1 {
      font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
        "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
        color: #2C2D35;
      font-size: 60px;
      line-height: 70px;
      overflow-y: hidden;
      span{
       color: #598d66;
      }
    }
    h2{
      font-size: 20px;
      line-height: 30px;
      color: #86928B;
    }
     button {
        outline: none;
        border: solid 1px #598D66;
        background-color: inherit;
        font-family: "Lucida Sans", "Lucida Sans Regular", "Lucida Grande",
          "Lucida Sans Unicode", Geneva, Verdana, sans-serif;
        font-size: 25px;
        color: #598D66;
        padding: 20px, 60px, 20px, 60px;
        gap: 10px;
        margin-top: 50px;
        width: 250px;
        height: 80px;
     }
  }
}
</style>