<template>
  <div id="home">
    <BaseImage
      source="ryan_camp_melenzana_blue.jpeg"
      alternate-text="Ryan Camp in blue melenzana smiling at February 2020 Turing Code Fair."
      size="large"
      display="circle"
      :border="true"
    />
    <h1>Ryan Camp</h1>
  </div>
</template>

<script>
import BaseImage from "@/components/BaseImage.vue";

export default {
  name: "Home",
  components: {
    BaseImage
  }
};
</script>

<style scoped>
#home {
  display: grid;
  align-items: center;
  justify-items: center;
}
#home h1 {
  align-self: start;
}
</style>
