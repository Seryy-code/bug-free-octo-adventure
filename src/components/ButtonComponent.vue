<template>
  <button @click="toggleText" :class="{ clicked: isClicked }">
    {{ editText }}
  </button>
</template>

<script>
export default {
  name: "ButtonComponent",
  data() {
    return {
      isClicked: false,
    };
  },
  computed: {
    editText() {
      return this.isClicked ? "text - 2" : "text - 1";
    },
  },
  methods: {
    toggleText() {
      this.isClicked = !this.isClicked;
    },
  },
};
</script>

<style scoped></style>
