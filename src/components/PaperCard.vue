<script setup lang="ts">
defineProps({
  title: {
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
    <div class="absolute top-0 custom-font px-12 pt-12 flex flex-row items-center gap-5">
      <img class="image" v-if="imagePath" :src="imagePath" />
      <div class="flex flex-col">
        <span class="text-4xl">{{title}}</span>
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
  height: 100px;
  width: auto;
}
</style>
