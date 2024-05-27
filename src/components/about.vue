<template>
  <div class="about">
    <div class="about__img">
      <div class="about__img-rama">
        <img src="../assets/about/rama.png" alt="rama" />
      </div>

      <div class="about__img-arm">
        <img src="../assets/about/arm.png" alt="arm" />
      </div>
    </div>
    <div class="about__aboutUS">
      <h5>Наша команда</h5>
      <span
        >Значимость этих проблем настолько очевидна, что базовый вектор развития
        позволяет оценить значение экспериментов, поражающих по своей
        масштабности и грандиозности. Мы вынуждены отталкиваться от того, что
        консультация с широким активом.</span
      >
      <div class="about__aboutUS-images">
        <img src="../assets/about/first.png" alt="first" />
        <img src="../assets/about/second.jpg" alt="second" />
        <img src="../assets/about/third.jpg" alt="third" />
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "aboutComponent",
});
</script>

<style scoped lang="scss">
.about {
  display: flex;
  height: 574px;
  width: 1440px;
  margin: auto;
  position: relative;
  margin-top: 50px;

  .about__img {
    width: 40%;
    height: max-content;
    display: grid;
    position: relative;
    padding-top: 50px;
  }
  .about__img-rama {
    grid-column: 1;
    grid-row: 1;
    padding-top: 70px;
    z-index: 1;
    width: 100%;
    img {
      width: 500px;
    }
  }
  .about__img-arm {
    grid-column: 1;
    grid-row: 1;
    z-index: 2;
    margin-left: 55px;
    margin-top: -30px;
    img {
      width: 310px;
    }
  }
  .about__aboutUS {
    width: 50%;
    height: auto;
    display: flex;
    flex-direction: column;
    justify-content: center;
    h5 {
      font-family: base-font;
      color: #2c2d35;
      font-size: 40px;
      line-height: 90px;
      font-weight: 500;
    }
    span {
      font-family: base-font;
      color: #2c2d35;
      font-size: 18px;
      line-height: 28px;
      font-weight: 500;
      text-align: left;
    }
    .about__aboutUS-images{
      display: flex;
      margin-top: 20px;
      gap: 20px;
    }
  }
}
</style>