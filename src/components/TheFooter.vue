<template>
  <div id="footer">
    <a href="https://www.linkedin.com/in/campprg">
      <BaseImage
        source="linked_in_logo.png"
        alternat-text="Linked in logo leading to Ryan Camp's Profile."
        size=""
        display=""
      />
    </a>
    <p>campryan@comcast.net</p>
  </div>
</template>

<script>
import BaseImage from "@/components/BaseImage";

export default {
  name: "TheFooter",
  components: {
    BaseImage
  }
};
</script>

<style scoped>
#footer {
  color: #f6c90e;
  background-color: #3a4750;
  display: grid;
  grid-template-columns: repeat(3, auto);
  justify-content: center;
}
p {
  margin: 0;
  padding-top: 0.4em;
  font-weight: bold;
  font-size: 1.2em;
}
</style>
