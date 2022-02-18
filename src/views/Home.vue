<template>
  <div class="flex">
    <div class="logo w-1/2 p-4">
      <img class="rounded" src="@/assets/img/logo-torres.png" alt="" />
    </div>
    <div class="w-1/2 p-4 font-extrabold text-3xl mt-48 text-center">
      <p class="uppercase text-white">
        {{ title }}
        <a
          class="text-red hover:underline hover:text-yellow-700"
          rel="nofollow noopener"
          href="https://l.facebook.com/l.php?u=https%3A%2F%2Fplay.google.com%2Fstore%2Fapps%2Fdetails%3Fid%3Dc3.amorocho.arvi%26fbclid%3DIwAR3xq-EXFNKUjaP-NSBxYQX2yArt9PgeqY5zLc2NIXeVFuJC-2x8zyluRVw&h=AT0HJrWjxbwWP6ieAgJ-KRZYgd_fAO8tXIAs4RN9hBUuh8xTYP8_yA_4cA7pWv2bpYeFAOTfzZGzvrYd2ecVobWcp1V28GtJ2YhRR3VLc0B4y-57hnbfyiMlBg&__tn__=%2CmH-R&c[0]=AT35HpgPiz7u3oBrax-LN3cJCuDSnFgXa4HkSZ5_x7HUC9Nlp-scSSXk8vaj7WCRINxq--FK1oAE0dMoIKIehe8W2vHwNocNkAij3EJoKQOapHk1C1FE4i1XAL-efGfQbfW00jKnz0fdwsFTOaahmC1Y"
          target="_blank"
          ><p class="text-lg">o desde la App Movil Arvi Internacional</p>
        </a>
      </p>
      <div class="flex justify-center py-4">
        <Audio />
      </div>
      <hr />
      <div class="mt-10">
        <p class="text-white text-sm text-center mb-3">Encuentranos en:</p>
        <div class="flex justify-center">
          <a href="https://www.facebook.com/arvismaquina.armandovilla" class="mr-6 text-white" target="_blank">
            <svg aria-hidden="true" focusable="false" data-prefix="fab" data-icon="facebook-f"
              class="w-4" role="img" xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 320 512">
              <path fill="currentColor"
                d="M279.14 288l14.22-92.66h-88.91v-60.13c0-25.35 12.42-50.06 52.24-50.06h40.42V6.26S260.43 0 225.36 0c-73.22 0-121.08 44.38-121.08 124.72v70.62H22.89V288h81.39v224h100.17V288z">
              </path>
            </svg>
          </a>
          <a href="https://www.instagram.com/arvi_internacional/" class="mr-6 text-white" target="_blank">
            <svg aria-hidden="true" focusable="false" data-prefix="fab" data-icon="instagram"
              class="w-6" role="img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 448 512">
              <path fill="currentColor"
                d="M224.1 141c-63.6 0-114.9 51.3-114.9 114.9s51.3 114.9 114.9 114.9S339 319.5 339 255.9 287.7 141 224.1 141zm0 189.6c-41.1 0-74.7-33.5-74.7-74.7s33.5-74.7 74.7-74.7 74.7 33.5 74.7 74.7-33.6 74.7-74.7 74.7zm146.4-194.3c0 14.9-12 26.8-26.8 26.8-14.9 0-26.8-12-26.8-26.8s12-26.8 26.8-26.8 26.8 12 26.8 26.8zm76.1 27.2c-1.7-35.9-9.9-67.7-36.2-93.9-26.2-26.2-58-34.4-93.9-36.2-37-2.1-147.9-2.1-184.9 0-35.8 1.7-67.6 9.9-93.9 36.1s-34.4 58-36.2 93.9c-2.1 37-2.1 147.9 0 184.9 1.7 35.9 9.9 67.7 36.2 93.9s58 34.4 93.9 36.2c37 2.1 147.9 2.1 184.9 0 35.9-1.7 67.7-9.9 93.9-36.2 26.2-26.2 34.4-58 36.2-93.9 2.1-37 2.1-147.8 0-184.8zM398.8 388c-7.8 19.6-22.9 34.7-42.6 42.6-29.5 11.7-99.5 9-132.1 9s-102.7 2.6-132.1-9c-19.6-7.8-34.7-22.9-42.6-42.6-11.7-29.5-9-99.5-9-132.1s-2.6-102.7 9-132.1c7.8-19.6 22.9-34.7 42.6-42.6 29.5-11.7 99.5-9 132.1-9s102.7-2.6 132.1 9c19.6 7.8 34.7 22.9 42.6 42.6 11.7 29.5 9 99.5 9 132.1s2.7 102.7-9 132.1z">
              </path>
            </svg>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { defineAsyncComponent, defineComponent } from "vue";

export default defineComponent({
  name: "Home",
  components: {
    Audio: defineAsyncComponent(() => import("@/components/Audio.vue")),
  },
  setup() {
    const title = "Escucha nuestra transmisión en vivo";
    return {
      title,
    };
  },
});
</script>
<style scoped>
.logo {
  @apply w-2/4 h-auto ml-4 rounded;
}

div {
  @apply bg-black
}
</style>
