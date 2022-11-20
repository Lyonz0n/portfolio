<script setup lang="ts">
import PaperCard from '../components/PaperCard.vue'

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
  <div class="game-card-container">
    <div id="card-1" class="absolute"><PaperCard :title="title" :image-path="imagePath"/></div>
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
  cursor: pointer;
  transform: scale(1);
  transition: 0.25s all ease;
}

#card-2 {
  z-index: 10;
  margin-top: 25px;
  margin-left: 25px;
  cursor: pointer;
  transform: scale(1);
  transition: 0.25s all ease;
}

#card-3 {
  margin-top: 45px;
  margin-left: -25px;
  cursor: pointer;
  transform: scale(1);
  transition: 0.25s all ease;
}
#card-1:hover {
  transform: scale(1.2);
}

#card-1:hover ~ #card-2{
  transform: scale(1.2);
}

#card-1:hover ~ #card-3{
  transform: scale(1.2);
}
</style>
