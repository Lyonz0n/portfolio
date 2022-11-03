<script setup lang="ts">
import PaperCard from '../components/PaperCard.vue'
import Img from "@/assets/castle.png"
</script>

<template>
  <div class="game-card-container">
    <div id="card-1" class="absolute"><PaperCard title="Kingdom Rivality" description="Jeu de stratégie en 1v1. Aurez la puissance nécessaire pour détruire votre adversaire et conquérir le trone ?" :image-path="Img"/></div>
    <div id="card-2" class="absolute move"><PaperCard/></div>
    <div id="card-3" class="absolute"><PaperCard/></div>
  </div>
</template>

<style scoped>
.game-card-container{
  position: relative;
  width: 530px;
  height: 300px;
}
#card-1 {
  z-index: 20;
  transition: margin-top 0.25s;
  cursor: pointer;
}

#card-2 {
  z-index: 10;
  transition: margin-left 0.25s,margin-top 0.25s;
  margin-top: 25px;
  margin-left: 25px;
  cursor: pointer;
}

#card-3 {
  transition: margin-left 0.25s,margin-top 0.25s;
  margin-top: 45px;
  margin-left: -25px;
  cursor: pointer;
}
#card-1:hover {
  margin-top: -10px;
}

#card-1:hover ~ #card-2{
  margin-top: 30px;
  margin-left: 30px;
}

#card-1:hover ~ #card-3{
  margin-top: 55px;
}
</style>
