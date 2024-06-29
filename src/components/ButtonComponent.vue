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

<style scoped>
button {
  padding: 10px 20px;
  font-size: 16px;
  cursor: pointer;
}
.clicked {
  background-color: #4caf50; /* Зеленый фон */
  color: white; /* Белый текст */
  transition: 0.1s ease-in;
}
</style>
