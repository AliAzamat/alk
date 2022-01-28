<template>
  <section class="reviews">
    <div class="container">
      <div class="reviews__row">
        <Item />
        <Item />
        <Item />
        <Item />
      </div>
    </div>
  </section>
</template>

<script>
import Item from "./Item.vue";
export default {
  components: { Item },
};
</script>

<style>
.reviews {
  background: #fff;
  padding: 80px 0;
}
.reviews__row {
  display: flex;
}
.reviews-item {
  width: 25%;
  text-align: center;
}
</style>