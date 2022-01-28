<template>
  <div class="reviews-item">
    <img :src="reviewsIcon" alt="" />
    <TagH type="h5">Заголовок #1</TagH>
    <p>Небольшое описание в 2 строчки</p>
  </div>
</template>

<script>
import TagH from "@/components/TagH/TagH.vue";
import reviewsIcon from "@/assets/review-item-1.svg";
export default {
  components: { TagH },
  data() {
    return {
      reviewsIcon,
    };
  },
};
</script>

<style>
.reviews-item h5 {
  margin: 35px 0 15px;
}
</style>