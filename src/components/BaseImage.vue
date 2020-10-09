<template>
  <div class="base-image">
    <p>{{style}}</p>
    <img
      :src="source_path"
      :alt="alternateText"
      :class="{
        small: size === 'small',
        medium: size === 'medium',
        large: size === 'large',
        rounded: display === 'rounded',
        circle: display === 'circle'
      }"
    />
  </div>
</template>
<script>
export default {
  name: "BaseImage",
  props: {
    source: String,
    alternateText: String,
    size: String,
    display: String
  },
  computed: {
    source_path() {
      return require(`@/assets/${this.source}`);
    }
  }
};
</script>
<style scoped>
img {
  height: auto;
  border: 2px solid black;
}
.small {
  width: 10em;
}
.medium {
  width: 15em;
}
.large {
  width: 20em;
}
.rounded {
  border-radius: 20%;
}
.circle {
  border-radius: 50%;
}
</style>
