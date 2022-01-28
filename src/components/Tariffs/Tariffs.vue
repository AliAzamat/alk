<template>
  <section class="tariffs">
    <div class="container">
      <TagH className="tariffs__title" type="h2">Тарифы</TagH>
      <div class="tariffs__row">
        <Item
          v-for="color in colors"
          :key="color"
          :style="{ background: color }"
        />
      </div>
    </div>
  </section>
</template>

<script>
import TagH from "@/components/TagH/TagH.vue";
import Item from "./Item.vue";
export default {
  components: { Item, TagH },
  data() {
    return {
      colors: ["#93E7FF", "#FFD773", "#A3A3FF", " #D1CAFF"].sort(
        () => Math.random() - 0.5
      ),
    };
  },
};
</script>

<style>
.tariffs {
  padding: 80px 0;
  background: linear-gradient(0deg, #F5F7F9, #F5F7F9), #ECE8E5;
}
.tariffs__row {
  display: flex;
}
.tariffs__title {
  margin-bottom: 45px;
}
.tariffs-item {
  margin-right: 20px;
  width: 25%;
  background: #93e7ff;
  border-radius: 20px;
  padding: 40px 20px 20px;
  text-align: center;
}
.tariffs-item:last-child {
  margin-right: 0;
}
.tariffs-item img {
  margin: 0 0 30px;
}
.tariffs-item h5 {
  margin-bottom: 30px;
}
.tariffs-item__price {
  display: inline-block;
  font-family: Gilroy;
  font-style: normal;
  font-weight: 600;
  font-size: 18px;
  line-height: 21px;
  color: #000000;
  margin: 15px 0 25px;
}
.tariffs-item__description {
  font-family: Gilroy;
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  line-height: 16px;
  color: #000000;
}
</style>