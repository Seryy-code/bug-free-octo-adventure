<template>
  <ol>
    <li v-for="(item, index) in list" :key="index">{{ item }}</li>
  </ol>
</template>
<script>
export default {
  name: "ListComponent",
  data() {
    return {
      list: ["Orange", "Apple", "Banana", "Kiwi", "Lime"],
    };
  },
};
</script>
<style scoped>
ol {
  width: 100px;
  text-align: center;
}
ol li {
  border-bottom: 1px solid black;
}
ol li:last-child {
  border: none;
}
</style>
