<template>
  <div class="home">
    <Navbar />
    <HelloWorld msg="Emisora Arvi"/>
  </div>
</template>

<script lang="ts">
import { defineAsyncComponent, defineComponent } from 'vue';

export default defineComponent({
  name: 'Home',
  components: {
    Navbar: defineAsyncComponent(() =>
      import('@/components/layouts/Navbar.vue')
    )
  },
});
</script>
