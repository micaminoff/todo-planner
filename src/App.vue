<template>
  <Header></Header>
  <div id="application">
      <Sidebar :items="itemList"></Sidebar>
      <Plan :items="itemList"></Plan>
  </div>
</template>

<script>
import { ref } from "vue";
import Header from "./components/Header.vue";
import Sidebar from "./components/Sidebar.vue";
import Plan from "./components/Plan.vue";

const itemList = [
  {
    id: 0,
    title: "Learn Vue.js",
    description: "Make a todo application.",
  },
  {
    id: 1,
    title: "Deploy",
    description: "Try out netlify.",
  },
  {
    id: 2,
    title: "Accessibility",
    description: "Learn and implement basic accessibility standards.",
  },
];

export default {
  name: "App",
  components: {
    Header,
    Sidebar,
    Plan,
  },
  setup() {
    return { itemList: ref(itemList) };
  },
};
</script>

<style scoped>
#application {
  display: flex;
  max-width: 90%;
  margin: 20px auto 0 auto;
  align-items: baseline;
  justify-content: space-evenly;
}
</style>
