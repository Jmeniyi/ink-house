<template>
  <mainPage/>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import mainPage from './pages/mainPage.vue';

export default defineComponent({
  name: 'App',
  components: {
    mainPage
  }
});
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  overflow-x: hidden;
}
</style>
