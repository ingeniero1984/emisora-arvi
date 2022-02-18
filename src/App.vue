<template>
  <Navbar />
  <router-view/>
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
