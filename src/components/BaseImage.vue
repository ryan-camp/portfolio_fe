<template>
  <div class="base-image">
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
    source: {
      type: String,
      required: true
    },
    alternateText: {
      type: String,
      require: true
    },
    size: {
      type: String,
      required: false,
      default: "medium"
    },
    display: {
      type: String,
      required: false,
      default: "rounded"
    }
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
  border: 0.15em solid #3a4750;
}
.small {
  max-width: 10em;
}
.medium {
  max-width: 20em;
}
.large {
  max-width: 30em;
}
.rounded {
  border-radius: 10%;
}
.circle {
  border-radius: 50%;
}
@media screen and (max-width: 800px) {
  img {
    width: 20em;
  }
}
@media screen and (max-width: 600px) {
  img {
    width: 10em;
  }
}
</style>
