<script setup lang="ts">
</script>

<template>
  <div class="frame items-center flex flex-col gap-10">
    <span class="text-4xl custom-font">Wanted</span>
    <img style="margin-right: 30px" src="@/assets/knight.png" />
    <span class="text-3xl custom-font">Louison Martin</span>

  </div>
</template>

<style scoped>
.frame {
  background-color: #fffef0;
  border: solid 5vmin #553C2A;
  border-bottom-color: #5e432e;
  border-left-color: #553C2A;
  border-radius: 2px;
  border-right-color: #553C2A;
  border-top-color: #4d3627;
  box-shadow:0 0 125px #8f5922 inset, 0 5px 10px 5px rgba(0, 0, 0, .25);
  box-sizing: border-box;
  margin: 10vh 10vw;
  width: 600px;
  height: 700px;
  padding: 3rem;
  position: relative;
  text-align: center;
  animation: wave ease-in-out 2s 1 alternate;
}

.frame:before {
   border-radius:2px;
   bottom:-2vmin;
   box-shadow:0 2px 5px 0 rgba(0,0,0,.25) inset;
   content:"";
   left:-2vmin;
   position:absolute;
   right:-2vmin;
   top:-2vmin;
}

frame:after {
   border-radius:2px;
   bottom:-2.5vmin;
   box-shadow: 0 2px 5px 0 rgba(0,0,0,.25);
   content:"";
   left:-2.5vmin;
   position:absolute;
   right:-2.5vmin;
   top:-2.5vmin;
}

@keyframes wave {
  0% { transform: rotate(0deg); }
  20% { transform: rotate(8deg); }
  40% { transform: rotate(-8deg); }
  60% { transform: rotate(5deg); }
  80% { transform: rotate(-5deg); }
  100% { transform: rotate(0deg); }
}
</style>
