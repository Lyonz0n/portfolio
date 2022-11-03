<script setup lang="ts">
</script>

<template>
  <div class="frame flex flex-col">
    <div class="frame-border-background frame-border-x"></div>
    <div class="flex flex-row flex-auto">
      <div class="frame-border-background frame-border-y"></div>
      <div class="flex-auto frame-content"></div>
      <div class="frame-border-background frame-border-y"></div>
    </div>
    <div class="frame-border-background frame-border-x"></div>
  </div>
</template>

<style scoped>
.frame {
  width: 600px;
  height: 700px;
  box-shadow: 8px 8px 15px rgba(0, 0, 0, 0.62);
}

.frame-content {
  box-shadow: 0 0 50px rgba(0, 0, 0, 0.80) inset;
}
.frame-border-background {
  background-color: #221812;
}
.frame-border-x {
  height: 50px;
  width: 100%;
}

.frame-border-y {
  width: 50px;
  height: 100%;
}
</style>
