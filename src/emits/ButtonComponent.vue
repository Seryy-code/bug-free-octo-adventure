<template>
  <button @click="sendData">edit figure</button>
</template>
<script setup>
import { defineEmits } from "vue";

const emit = defineEmits(["sendEditFigure"]);
function sendData() {
  emit("sendEditFigure");
  console.log("send signal...");
}
</script>
<style></style>
