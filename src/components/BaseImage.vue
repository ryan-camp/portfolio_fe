<template>
  <div class="base-image">
    <img
    :src="source_path"
    :alt="alternateText"
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
    style: String
  },
  computed: {
    source_path() {
      return require(`@/assets/${this.source}`)
    }
  }
};
</script>
<style scoped>
</style>
