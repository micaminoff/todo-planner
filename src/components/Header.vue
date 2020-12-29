<template>
  <header>
    <div>
      <p>Logo & name</p>
      <nav>
        <p>WIP</p>
        <p>About</p>
        <a href="#">Login</a>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
header {
  background-color: red;
  width: 95%;
  height: 30px;
  padding: 15px 0;
  border-radius: 10px;
  margin: 30px auto 0;
}
div {
  margin: 0 15px;
  height: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
div > p {
  max-height: 90%;
  height: auto;
  background-color: darkred;
  color: white;
  padding: 15px;
}
nav {
  display: flex;
  height: 100%;
  background-color: darkred;
}
nav > * {
  background-color: black;
  margin: 0 15px;
  padding: 5px;
  color: white;
  max-height: 90%;
}
</style>
