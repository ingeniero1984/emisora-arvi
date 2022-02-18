<template>
  <div class="mt-4">
    <Card />
  </div>
</template>

<script lang="ts">
import { defineAsyncComponent, defineComponent } from 'vue';

export default defineComponent({
  name: 'Events',
    components: {
    Card: defineAsyncComponent(() =>
      import('@/components/Card.vue')
    )
  },
});
</script>

<style scoped>
div {
  @apply bg-black
}
</style>
