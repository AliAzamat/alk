<template>
  <div class="portfolio-item">
    <img :src="{ imgUrl }" />
    <TagH type="h5">{{ title }}</TagH>
    <span>{{ link }}</span>
  </div>
</template>

<script>
import TagH from "@/components/TagH/TagH.vue";
export default {
  props: ["title", "link", "imgUrl"],
  components: { TagH },
  data() {
    return {};
  },
};
</script>

<style>
</style>