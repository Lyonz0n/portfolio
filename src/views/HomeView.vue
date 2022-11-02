<script setup lang="ts">
import PaperCard from '../components/PaperCard.vue'
</script>

<template>
  <div class="w-full flex flex-row justify-center">
    <div class="page-container">
        <PaperCard></PaperCard>
        <PaperCard></PaperCard>
    </div>
  </div>
</template>

<style scoped>
.page-container {
  width: 1300px;
}
</style>
