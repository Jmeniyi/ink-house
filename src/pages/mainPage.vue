<template>
<headerComponent/>
<hero-component/>
<catalogComponent/>
<promoComponent/>
<aboutComponent/>
<footerComponent/>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

import headerComponent from '@/components/header.vue'
import heroComponent from '@/components/hero.vue'
import catalogComponent from '@/components/catalog.vue'
import promoComponent from '@/components/promo.vue'
import aboutComponent from '@/components/about.vue'
import footerComponent from '@/components/footer.vue'

export default defineComponent({
  name: 'Main-Page',
  components:{
    headerComponent,
    heroComponent,
    catalogComponent,
    promoComponent,
    aboutComponent,
    footerComponent
  }
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
