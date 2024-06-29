<template>
  <div class="cont">
    <input type="num" v-model="num1" />
    <input type="num" v-model="num2" />
  </div>
  <p>[{{ num1 }}] - [{{ num2 }}] = [{{ res }}]</p>
</template>
<script setup>
import { ref, computed } from "vue";

const num1 = ref(0);
const num2 = ref(0);
const res = computed(() => num1.value - num2.value);
</script>
<style scoped>
.cont {
  display: flex;
}
</style>
