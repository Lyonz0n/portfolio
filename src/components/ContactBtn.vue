<script setup lang="ts">
</script>

<template>
  <a href="https://twitter.com/a_croquelois" target="_blank" class="position-relative contact-btn">
    <div class="content-btn flex flex-row justify-center items-center px-4 py-4 rounded-xl cursor-pointer position-relative gap-3 absolute">
      <span class="text-3xl custom-font text-light">Contactez-moi</span>
      <img class="image" src="@/assets/pigeon.png" />
    </div>
    <div class="contour-btn rounded-xl absolute" />
  </a>
</template>

<style scoped>
.contact-btn {
  width: 390px;
  height: 113px;
}

.contour-btn {
  width: 390px;
  height: 113px;
  z-index: -1;
  margin-left: 5px;
  margin-top: 5px;
  background-color: #2d1e16;
  box-shadow: 2px 2px 15px rgba(0, 0, 0, 0.68)
}

.content-btn {
  width: 390px;
  z-index: 5;
  background-color: #362419;
  transition: 0.25s all ease;
}

.content-btn:hover {
  transform: translate(5px, 5px);
}

.image {
  width: 80px;
  height: auto;
}
</style>
