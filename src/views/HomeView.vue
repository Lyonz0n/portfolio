<script setup lang="ts">
import GameCard from "@/components/GameCard.vue";
import Wanted from "@/components/Wanted.vue";
import ContactBtn from "@/components/ContactBtn.vue";
</script>

<template>
  <div class="app-container flex flex-row">
    <div class="flex-1 flex flex-col items-center justify-center">
      <Wanted/>
      <ContactBtn class="mt-28"/>
    </div>
    <div class="flex-1 flex flex-col items-center justify-center">
      <GameCard title="Projets" image-path="./images/idea.png"/>
      <GameCard title="Références" image-path="./images/reference.png"/>
    </div>
  </div>
</template>

<style scoped>
.app-container {
  width: 100%;
  height: 100vh;
}
</style>
