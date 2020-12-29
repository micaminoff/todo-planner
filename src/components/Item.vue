<template>
  <div id="item">
    <h1>{{ title }}</h1>
    <p>{{ description }}</p>
    <p>Done: {{ done }}</p>
  </div>
</template>

<script>
export default {
  name: "Item",
  props: {
    title: String,
    description: String,
  },
  data() {
    return {
      done: false,
    };
  },
};
</script>

<style scoped>
  #item {
    background-color: black;
  }
</style>
