<template>
  <div class="font-sans antialiased" id="app">
  <nav class="flex justify-between flex-wrap bg-gray-800 p-6 text-right">
    <div class="flex items-center flex-no-shrink text-white mr-6">
      <span class="font-semibold text-xl tracking-tight">Tailwind CSS</span>
    </div>
    <div class="block sm:hidden">
      <button @click="toggle" class="flex items-center px-3 py-2 border rounded text-teal-lighter border-teal-light hover:text-white hover:border-white">
        <svg class="fill-current h-3 w-3" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><title>Menu</title><path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"/></svg>
      </button>
    </div>
    <div :class="open ? 'block': 'hidden'" class="w-full flex-grow sm:flex sm:items-center sm:w-auto">
      <div class="text-sm sm:flex-grow">
        <a href="#responsive-header" class="no-underline block mt-4 sm:inline-block sm:mt-0 text-teal-lighter hover:text-white mr-4">
          Docs
        </a>
        <a href="#responsive-header" class="no-underline block mt-4 sm:inline-block sm:mt-0 text-teal-lighter hover:text-white mr-4">
          Examples
        </a>
        <a href="#responsive-header" class="no-underline block mt-4 sm:inline-block sm:mt-0 text-teal-lighter hover:text-white">
          Blog
        </a>
      </div>
    </div>
  </nav>
</div>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue'

export default defineComponent({
    name: 'Navbar',
    setup() {
        const open = ref<boolean>(false)
        
        const toggle = () => {
            open.value = !open.value
        }

        return {
            open, toggle
        }
    }
})
</script>

<style>

</style>