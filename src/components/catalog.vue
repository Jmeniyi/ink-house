<template>
  <div class="catalog">
    <div class="catalog__filters">
      <span>Репродукции</span>
      <div class="catalog__filters-toggle">
        <button>Франция</button>
        <button>Германия</button>
        <button>Англия</button>
      </div>
    </div>
    <div class="catalog__products">
      <div
        class="catalog__products-product"
        v-for="(item, i) in data.items"
        :key="i"
      >
        <img v-if="item.picture" :src="item.picture" alt="Изображение" />
        <h2>{{ item.author }}</h2>
        <h1>{{ item.nameComposition }}</h1>
        <h3>{{ item.typeSize }}</h3>
        <h4>{{ item.price }}</h4>
        <button>В корзину</button>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import data from "../assets/dataCatalog.json";

export default defineComponent({
  name: "catalogComponent",
  data() {
    return {
      data,
    };
  },
});
</script>

<style scoped lang="scss">

.catalog {
  margin: auto;
  margin-top: 40px;
  margin-bottom: 40px;
  width: 1440px;
  gap: 45px;

  .catalog__filters {
    display: flex;
    align-items: center;
    span {
     
      color: #2c2d35;
      font-size: 40px;
      line-height: 62px;
      overflow-y: hidden;
    }
    .catalog__filters-toggle {
      display: flex;
      justify-content: end;
      gap: 40px;
      margin-left: auto;

      button {
        width: auto;
        margin-top: 10px;
        margin-bottom: 10px;
        border-radius: 20px;
        padding: 10px 20px 10px 20px;
        font-family: base-font;
        color: #2c2d35;
        font-weight: 500;
        font-size: 25px;
        line-height: 32px;
        background-color: #d4e8d9;
        color: #2c2d35;
        border: 2px solid #d4e8d9;
        cursor: pointer;
      }
      button:active {
        background-color: #376b44;
        color: #f4f6f5;
        border: 2px solid #376b44;
      }
      button:focus {
        background-color: #D4E8D9;
        color: #2C2D35;
        border: 2px solid #598D66;
      }
      button:hover {
        background-color: #598D66;
        color: #f4f6f5;
      }
    }
  }
  .catalog__products {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    margin-top: 20px;
    gap: 10px;
    .catalog__products-product {
      width: auto;
      overflow: visible;
      padding: 30px;
      background-color: #e1ede6;
      margin-bottom: 20px;
      img {
        max-width: 350px;
        height: 482px;
      }
      h2 {
        color: #86928b;
        font-size: 18px;
        font-family: base-font;
        font-weight: 500;
        line-height: 22px;
        margin-top: 7px;
      }
      h1{
        color: #2C2D35;
        font-size: 30px;
        font-family: base-font;
        font-weight: 500;
        line-height: 36px;
        margin-top: 10px;
      }
      h3{
        color: #2C2D35;
        font-size: 18px;
        font-family: base-font;
        font-weight: 500;
        line-height: 22px;
        margin-top: 10px;
      }
      h4{
        color: #598D66;
        font-size: 24px;
        font-family: base-font;
        font-weight: 500;
        line-height: 28px;
        margin-top: 7px;
      }
      button{
        width: 350px;
        margin-top: 20px;
        padding: 10px 20px 10px 20px;
        font-family: base-font;
        color: #2c2d35;
        font-weight: 500;
        font-size: 25px;
        line-height: 32px;
        background-color: #e1ede6;
        color: #598D66;
        border: 1px solid #598D66;
        gap: 6px;
        cursor: pointer;
      }
      button:active {
        background-color: #376b44;
        color: #f4f6f5;
      }
      button:focus {
        background-color: #D4E8D9;
        color: #2C2D35;
      }
      button:hover {
        background-color: #598D66;
        color: #f4f6f5;
      }
    }
  }
}
</style>