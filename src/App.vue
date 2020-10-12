<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view />
  </div>
</template>

<style>
#app {
  font-family: ABeeZee, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #303841;
}
/* primary     #303841
   secondary   #3a4750
   tertiary    #f6c90e
   quaternary  #eeeeee */

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
