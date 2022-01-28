<template>
  <div class="footer-item">
    <TagH type="h5">{{ label }}</TagH>
    <ul class="footer-list">
      <li v-for="item in items" :key="item" class="footer-list__item">
        {{ item }}
      </li>
    </ul>
  </div>
</template>

<script>
import TagH from "@/components/TagH/TagH.vue";
export default {
  props: ["label", "items"],
  components: { TagH },
};
</script>

<style>
</style>