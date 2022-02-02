<template>
    <div>
        <audio class="audio" controls src="https://streaming.radiosenlinea.com.ar/8920/stream" />
    </div>
</template>

<script lang="ts">
import { defineComponent } from "@vue/runtime-core";

export default defineComponent({
    name: 'Audio'
})
</script>

<style>
.audio {
    @apply py-2 m-3
}
</style>