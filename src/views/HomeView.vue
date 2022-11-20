<script setup lang="ts">
import GameCard from "@/components/GameCard.vue";
import Wanted from "@/components/Wanted.vue";
import ContactBtn from "@/components/ContactBtn.vue";
</script>

<template>
  <div class="app-container flex flex-row">
    <div class="flex-1 flex flex-col items-center justify-center"><Wanted/></div>
    <div class="flex-1 flex flex-col items-center justify-center">
      <GameCard title="Projets" image-path="./images/idea.png"/>
      <GameCard title="Références" image-path="./images/reference.png"/>
      <ContactBtn  class="mt-20"/>
    </div>
  </div>
</template>

<style scoped>
.app-container {
  width: 100%;
  height: 100vh;
}
</style>
