<template>
  <div id="app">
    <TheNavbar />
    <router-view />
  </div>
</template>

<script>
import TheNavbar from "@/components/TheNavbar";

export default {
  name: "App",
  components: {
    TheNavbar
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #303841;
}
/* primary     #303841
   secondary   #3a4750
   tertiary    #f6c90e
   quaternary  #eeeeee */
</style>
