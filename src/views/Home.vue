<template>
  <div class="home">
    <BaseImage
      source="ryan_camp_melenzana_blue.jpeg"
      alternate-text="Ryan Camp in blue melenzana smiling at February 2020 Turing Code Fair."
      size="large"
      display="circle"
    />
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
