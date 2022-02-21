<template>
  <div class="navbar font-sans antialiased">
  <nav class="flex justify-between flex-wrap bg-gray-900 text-right py-4">
    <div class="flex items-center flex-no-shrink">
      <img class="w-full h-20 ml-8 cursor-pointer" src="@/assets/img/logo-arvi.png" alt="logo arvi"/>
    </div>
    <ul class="md:flex md:items-center mr-6">
      <li class="mx-4 my-2 md:my:0 text-lg text-yellow-600 hover:text-white cursor-pointer">
        <router-link :to="{ name: 'Home' }">INICIO</router-link>
      </li>
      <li class="mx-4 my-2 md:my:0 text-lg text-yellow-600 hover:text-white cursor-pointer">
        <router-link :to="{ name: 'Programation' }">PROGRAMACIÓN</router-link>
      </li>
      <li class="mx-4 my-2 md:my:0 text-lg text-yellow-600 hover:text-white cursor-pointer">
        <router-link :to="{ name: 'Events' }">EVENTOS</router-link>
      </li>
      <li class="mx-4 my-2 md:my:0 text-lg text-yellow-600 hover:text-white cursor-pointer">
        <router-link :to="{ name: 'Contact' }">CONTACTENOS</router-link>
      </li>
    </ul>
  </nav>
</div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'Navbar'
})
</script>

<style>

</style>