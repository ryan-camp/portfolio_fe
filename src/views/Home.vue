<template>
  <div class="home">
    <BaseImage
      source="logo.png"
      alternate-text="Ryan Camp in blue melenzana smiling at February 2020 Turing Code Fair."
      size="small"
      style="rounded"
    />
    <img alt="Vue logo" src="../assets/ryan_camp_melenzana_blue.jpeg" />

  </div>
</template>

<script>
// @ is an alias to /src
import BaseImage from "@/components/BaseImage.vue";

export default {
  name: "Home",
  components: {
    BaseImage
  }
};
</script>
