<template>
  <div class="figure" :class="{ active: getbool }"></div>
  <p>Данные isClicked: {{ getbool }}</p>
</template>

<script setup>
import { defineProps } from "vue";

defineProps({
  getbool: Boolean,
});
</script>

<style scoped>
.figure {
  position: absolute;
  top: 0;
  right: 0;
  transition: 0.3s ease;
  margin-top: 10px;
  width: 50px;
  height: 50px;
  background-color: gray;
}
.figure.active {
  width: 70px;
  height: 70px;
  background-color: brown;
  border-radius: 50%;
}
</style>
