<template>
  <div id="footer">
    <a id="linkedin-logo" href="https://www.linkedin.com/in/campprg">
      <BaseImage
        source="linked_in_logo.png"
        alternat-text="Linked in logo leading to Ryan Camp's Profile."
        size="tiny"
      />
    </a>

    <p>campryan@comcast.net</p>

    <a id="github-logo" href="https://github.com/cmpprg">
      <BaseImage
        source="github-mark-light.png"
        alternat-text="Github logo leading to Ryan Camp's Profile."
        size="tiny"
      />
    </a>
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
  border-radius: 25% 25% 0 0;
  display: grid;
  grid-template-columns: repeat(3, auto);
  justify-content: center;
  align-items: center;
  gap: 2em;
}
@media screen and (max-width: 800px) {
  #footer {
    border-radius: 0;
  }
}
p {
  margin: 0;
  padding-bottom: 0.4em;
  font-weight: bold;
  font-size: 1.2em;
}
</style>
