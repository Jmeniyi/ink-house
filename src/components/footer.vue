<template>
  <div class="footer">
    <div class="footer__first">
      <div class="footer__first-logo">
        <img alt="logo" src="../assets/logo.png" />
        <span>Ink. House</span>
      </div>
      <h5>+7 (999) 543-54-54</h5>
      <h6>Мастерская</h6>
    </div>
    <div class="footer-second">
      <h5>Репродукции</h5>
      <h6>Франция</h6>
      <h6>Германия</h6>
      <h6>Англия</h6>
    </div>
    <div class="footer-third">
      <h5>Новинки</h5>
      <h6>2021</h6>
      <h6>2022</h6>
    </div>
    <div class="footer-fourth">
      <h5>О нас</h5>
      <h6>Художники</h6>
      <h6>Менеджеры</h6>
    </div>
    <div class="footer-fifth">
      <div class="footer-fifth-social">
        <img src="../assets/footer/Frame.svg" alt="facebook" />
        <img src="../assets/footer/Frame2.svg" alt="instagram" />
        <img src="../assets/footer/Frame3.svg" alt="youtube" />
      </div>
      <span
        >Ink. House ® <br />
        All rights reserved</span
      >
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "footerComponent",
});
</script>

<style  scoped lang="scss">
.footer {
  height: 180px;
  background-color: rgba(225, 237, 230, 1);
  width: 1440px;
  margin: auto;
  display: grid;
  grid-template-columns: 25% 10% 10% 10% 25%;
  justify-content: center;
  align-content: center;
  justify-items: center;
  .footer__first {
    gap: 8px;
    display: flex;
    flex-direction: column;
    .footer__first-logo {
      gap: 8px;
      display: flex;
      align-items: center;
      margin-bottom: 20px;
    }
    img {
      height: 45px;
      width: 45px;
    }
    span {
      font-family: base-font;
      color: #598d66;
      font-size: 20px;
      font-weight: 500;
      line-height: 25px;
    }
    h5 {
      font-family: base-font;
      color: rgba(44, 45, 53, 1);
      font-size: 20px;
      line-height: 25px;
      font-weight: 500;
    }
    h6 {
      font-family: base-font;
      color: rgba(134, 146, 139, 1);
      font-size: 18px;
      line-height: 20px;
      font-weight: 500;
    }
  }
  .footer-second {
    gap: 8px;
    display: flex;
    flex-direction: column;
    h5 {
      font-family: base-font;
      color: rgba(44, 45, 53, 1);
      font-size: 20px;
      line-height: 25px;
      font-weight: 500;
    }
    h6 {
      font-family: base-font;
      color: rgba(134, 146, 139, 1);
      font-size: 18px;
      line-height: 27px;
      font-weight: 500;
    }
  }
  .footer-third {
    gap: 8px;
    display: flex;
    flex-direction: column;
    h5 {
      font-family: base-font;
      color: rgba(44, 45, 53, 1);
      font-size: 20px;
      line-height: 25px;
      font-weight: 500;
    }
    h6 {
      font-family: base-font;
      color: rgba(134, 146, 139, 1);
      font-size: 18px;
      line-height: 27px;
      font-weight: 500;
    }
  }
  .footer-fourth {
    gap: 8px;
    display: flex;
    flex-direction: column;
    h5 {
      font-family: base-font;
      color: rgba(44, 45, 53, 1);
      font-size: 20px;
      line-height: 25px;
      font-weight: 500;
    }
    h6 {
      font-family: base-font;
      color: rgba(134, 146, 139, 1);
      font-size: 18px;
      line-height: 27px;
      font-weight: 500;
    }
  }
  .footer-fifth {
    .footer-fifth-social {
      gap: 10px;
      display: flex;
      margin-bottom: 10px;
    }
    img {
      height: 25px;
      width: 25px;
    }
    span {
      font-family: base-font;
      color: rgba(44, 45, 53, 1);
      font-size: 12px;
      line-height: 25px;
      font-weight: 500;
    }
  }
}
</style>