<template>
  <div id="sidebar-container">
    <Category></Category>
    <Category></Category>
  </div>
</template>

<script>
import Category from './Category.vue'
export default {
    name: "Sidebar",
    components: {Category},
}
</script>

<style scoped>
  #sidebar-container {
    background-color: red;
    margin-top: 20px;
    padding: 10px;
  }
</style>