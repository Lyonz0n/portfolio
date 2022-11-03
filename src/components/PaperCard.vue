<script setup lang="ts">
defineProps({
  title: {
    type: String,
    default: ""
  },
  description: {
    type: String,
    default: ""
  },
  imagePath: {
    type: String,
    default: ""
  }
})
</script>

<template>
  <div class="relative paper-card-container">
    <div class="parchment w-full h-full relative">
    </div>
    <div class="absolute top-0 custom-font px-6 pt-10 flex flex-row items-center gap-5">
      <img class="image" v-if="imagePath" :src="imagePath" />
      <div class="flex flex-col">
        <span class="text-2xl">{{title}}</span>
        <span class="text-sm">{{description}}</span>
      </div>
    </div>
  </div>
</template>

<style scoped>
.paper-card-container {
  width: 480px;
  height: 200px;
}

.image {
  height: 120px;
  width: 120px;
}
</style>
