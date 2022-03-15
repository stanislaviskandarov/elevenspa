<template>
  <div class="container mx-auto">
    <Blog />
    <ImageSlider />
  </div>
</template>

<script>
import Blog from "../components/Blog";
import ImageSlider from "../components/ImageSlider";

export default {
  name: "HomePage",
  components: {
    Blog,
    ImageSlider,
  },
};
</script>

<style scoped>
</style>
