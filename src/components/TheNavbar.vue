<template>
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </div>
</template>

<script>
  export default {
    name: "TheNavbar"
  }
</script>

<style scoped>
  #nav {
    padding: 1.5rem;
    margin-bottom: 2%;
    background-color: #f6c90e;
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
