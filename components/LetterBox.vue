<script setup lang="ts">
const props = defineProps({
  letter: {
    type: String,
    default: ""
  },
  color: {
    type: String,
    default: "green"
  }
})
</script>

<template>
  <div class="col-span-1 flex items-center justify-center h-16 uppercase border-2 transition-all duration-300"
  :class="{
    'border-gray-500 bg-gray-500 text-white': color == 'gray',
    'border-green-500 bg-green-500 text-white': color == 'green',
    'border-yellow-500 bg-yellow-500 text-white': color == 'yellow'
  }">{{letter}}</div>
</template>

<style scoped>

</style>