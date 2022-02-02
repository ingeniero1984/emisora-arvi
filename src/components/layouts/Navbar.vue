<template>
  <div class="navbar font-sans antialiased">
  <nav class="flex justify-between flex-wrap bg-gray-800 text-right">
    <div class="flex items-center flex-no-shrink text-white mr-6">
      <!-- <img class="w-28 h-20 ml-4 cursor-pointer" src="@/assets/img/logo.png" alt="logo arvi"/> -->
      <h1 class="text-xl text-yellow-600 ml-6">{{ name }}</h1>
    </div>
    <Audio />
    <ul class="md:flex md:items-center mr-6">
      <li class="mx-4 my-2 md:my:0 text-sm text-white hover:text-yellow-600 cursor-pointer">
        <router-link :to="{ name: 'Home' }">Home</router-link>
      </li>
      <li class="mx-4 my-2 md:my:0 text-sm text-white hover:text-yellow-600 cursor-pointer">
        <router-link :to="{ name: 'Programation' }">Programación</router-link>
      </li>
      <li class="mx-4 my-2 md:my:0 text-sm text-white hover:text-yellow-600 cursor-pointer">
        <router-link :to="{ name: 'Events' }">Eventos</router-link>
      </li>
      <li class="mx-4 my-2 md:my:0 text-sm text-white hover:text-yellow-600 cursor-pointer">
        <router-link :to="{ name: 'Contact' }">Contactenos</router-link>
      </li>
    </ul>
  </nav>
</div>
</template>

<script lang="ts">
import { defineAsyncComponent, defineComponent } from 'vue'

export default defineComponent({
    name: 'Navbar',
    components: {
      Audio: defineAsyncComponent(() =>
      import('@/components/Audio.vue')
    )
    },
    setup () {
      const name = 'Organización Musical Arvi'

      return  { name }
    }
})
</script>

<style>

</style>