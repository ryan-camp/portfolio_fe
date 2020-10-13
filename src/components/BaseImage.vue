<template>
  <div class="base-image">
    <img
      :src="source_path"
      :alt="alternateText"
      :class="{
        tiny: size === 'tiny',
        small: size === 'small',
        medium: size === 'medium',
        large: size === 'large',
        rounded: display === 'rounded',
        circle: display === 'circle',
        border: border === true
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
      required: false
    },
    border: {
      type: Boolean,
      required: false,
      default: false
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
}
.border {
  border: 0.2em solid #3a4750;
}
.large {
  max-width: 30em;
}
@media screen and (max-width: 800px) {
  img {
    width: 20em;
  }
}

.medium {
  max-width: 20em;
}
@media screen and (max-width: 600px) {
  img {
    width: 10em;
  }
}

.small {
  max-width: 10em;
}
.tiny {
  max-width: 2em;
}
.rounded {
  border-radius: 10%;
}
.circle {
  border-radius: 50%;
}
</style>
