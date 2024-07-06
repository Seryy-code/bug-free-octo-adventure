<template>
  <div class="container">
    <ButtonComponent @sendEditFigure="receiveFigure"></ButtonComponent>
    <FigureComponent :getbool="isClicked"></FigureComponent>
  </div>
</template>
<script setup>
import { ref } from "vue";
import ButtonComponent from "./ButtonComponent.vue";
import FigureComponent from "./FigureComponent.vue";

let isClicked = ref(true);

function receiveFigure() {
  console.log("... signal received!");
  isClicked.value = !isClicked.value;
  console.log(isClicked.value);
}
</script>
<style scoped>
.container {
  position: relative;
  width: 500px;
}
</style>
