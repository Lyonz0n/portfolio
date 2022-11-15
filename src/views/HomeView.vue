<script setup lang="ts">
import GameCard from "@/components/GameCard.vue";
import Wanted from "@/components/Wanted.vue";
</script>

<template>
  <div class="w-full flex flex-row">
    <div class="flex-none"><Wanted/></div>
    <div class="flex-auto flex flex-col items-center justify-center">
      <GameCard id="game-1"/>
      <GameCard id="game-2"/>
      <GameCard id="game-3"/>
      <GameCard id="game-4"/>
      <GameCard id="game-5"/>
      <GameCard id="game-6"/>
    </div>
  </div>
</template>

<style scoped>
#game-1 {
  margin-left: 0;
}
#game-2 {
  margin-left: 100px;
}
#game-3 {
  margin-right: 200px;
}
#game-4 {
  margin-left: 0;
}
#game-5 {
  margin-right: 180px;
}
#game-6 {
  margin-left: 100px;
}
</style>
