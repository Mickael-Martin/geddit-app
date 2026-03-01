<template>
  <div>Compact Video Component</div>
</template>

<script>
export default {
  name: 'CompactVideo',
  mounted() {
    // Subscribe to HLS events here
  },
  beforeDestroy() {
    // Clean up HLS resources on component unmount
    if (this.hls) {
      this.hls.destroy();
    }
  }
};
</script>