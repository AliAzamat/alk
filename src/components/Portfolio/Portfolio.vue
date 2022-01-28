<template>
  <section class="portfolio">
    <div class="container">
      <TagH type="h2" className="portfolio__title">Н2 - ПОРТФОЛИО САЙТОВ</TagH>
      <div class="portfolio__row">
        <Item
          v-for="item in items"
          :key="item.id"
          :title="item.title"
          :link="item.link"
          :src="item.imgUrl"
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
      items: [
        {
          id: 1,
          title: "Продвижение по позициям",
          link: "ecutools.ru",
          imgUrl: "@/assets/portfolio-item-1.png",
        },
        {
          id: 2,
          title: "Продвижение по позициям",
          link: "ecutools.ru",
          imgUrl: "@/assets/portfolio-item-2.png"
        },
        {
          id: 3,
          title: "Продвижение по позициям",
          link: "ecutools.ru",
          imgUrl: "@/assets/portfolio-item-3.png"
        },
        {
          id: 4,
          title: "Продвижение по позициям",
          link: "ecutools.ru",
          imgUrl: "@/assets/portfolio-item-4.png"
        },
      ],
    };
  },
};
</script>

<style>
.portfolio {
  background: #fff;
}
.portfolio__title {
  margin: 85px 0 45px;
}
.portfolio__row {
  display: flex;
  margin-bottom: 80px;
}
.portfolio-item {
  width: 25%;
  background: #f5f7f9;
  border-radius: 20px;
  padding: 20px 20px 35px 20px;
  display: flex;
  flex-direction: column;
  margin-right: 20px;
}
.portfolio-item:last-child {
  margin-right: 0;
}
.portfolio-item h5 {
  text-align: left;
  margin: 30px 0 8px;
}
</style>