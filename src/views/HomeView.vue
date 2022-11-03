<script setup lang="ts">
import GameCard from "@/components/GameCard.vue";
import Wanted from "@/components/Wanted.vue";
</script>

<template>
  <div class="w-full flex flex-row">
    <div class="w-1/2 p-10"><Wanted /></div>
    <div class="w-1/2 flex flex-col items-center justify-center">
      <GameCard id="game-1"/>
      <GameCard id="game-2"/>
    </div>
  </div>
</template>

<style scoped>
#game-1 {
  margin-right: 100px;
}
#game-2 {
  margin-left: 100px;
}
</style>
