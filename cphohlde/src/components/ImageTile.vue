<script lang="ts" setup>
import {ref} from 'vue'
defineProps<{
  src: string
}>()
const hover = ref(false)
const isShifted = ref(false)
</script>
<template>
  <div class="relative h-full w-full object-cover" @mouseover="hover = true" @mouseleave="hover = false">
    <img :src="src" class="grayscale hover:grayscale-10 h-full w-full object-cover duration-500 group-hover:grayscale-0" @click="isShifted = !isShifted" :class="{'absolute z-10 w-quad h-quad object-cover': isShifted}" >


  <div v-if="hover" class="bg-black text-white opacity-60  w-full absolute flex bottom-0 left-0">
    <p class="text-white font-extralight">
      <slot/>
    </p>
  </div>
  </div>


</template>