<template>
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </div>
</template>

<script>
export default {
  name: "TheNavbar"
};
</script>

<style scoped>
#nav {
  background-color: #f6c90e;
  display: grid;
  grid-template-columns: auto auto auto;
  align-items: center;
  justify-content: center;
  gap: 1em;
}

#nav a {
  font-weight: bold;
  color: #303841;
  text-decoration: none;
  font-size: 1.5em;
}

#nav a.router-link-exact-active {
  color: #eeeeee;
  font-size: 2em;
}
</style>
