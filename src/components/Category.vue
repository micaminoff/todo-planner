<template>
  <div id="category-container">
    <h1>I'm a category!</h1>
    <Item title="item1" description="I am an item"></Item>
    <Item title="item2" description="I am another item"></Item>
  </div>
</template>

<script>
import Item from './Item.vue';
export default {
  name: "Category",
  components: {Item}
};
</script>

<style scoped>
#category-container {
  background-color: darkred;
  margin: 15px;
  padding: 5px;
  color: white;
  max-height: 90%;
  border: 1px solid black;
}
</style>
