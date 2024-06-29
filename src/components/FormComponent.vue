<template>
  <label for="">
    <input type="email" v-model="email" />
    <input type="password" v-model="password" />
  </label>
  <p id="email">email: {{ email }}</p>
  <p id="password">password: {{ password }}</p>
</template>
<script setup>
import { ref } from "vue";

const email = ref("");
const password = ref("");
</script>

<style></style>
