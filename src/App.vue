<script setup lang="ts">
import { RouterView } from 'vue-router'
</script>

<template>
  <RouterView />
  <svg>
    <filter id="wavy2">
      <feTurbulence x="0" y="0" baseFrequency="0.02" numOctaves="5" seed="1" />
      <feDisplacementMap in="SourceGraphic" scale="20" />
    </filter>
  </svg>
</template>

<style>
@font-face {
  font-family: "berry_rotunda";
  src: local("berry_rotunda"),
  url(./fonts/berry_rotunda.ttf) format("truetype");
}

body{
  background-color: #443022;
  background-image: url("./assets/background.png");
}
</style>
