<template>
  <footer class="footer">
    <div class="container">
      <div class="footer__row">
        <Logo />
        <Item label="Продвижение сайтов" :items="sitePromotion" />
        <Item label="Создание сайтов" :items="siteCreation" />
        <Item label="Контекстная реклама " :items="contextAdvert" />
      </div>
      <Bottom />
    </div>
  </footer>
</template>

<script>
import Logo from "./Logo.vue";
import Item from "./Item.vue";
import Bottom from "./FooterBottom.vue";
export default {
  components: { Logo, Item, Bottom },
  data() {
    return {
      sitePromotion: ["По позициям", "По трафику"],
      siteCreation: ["Визитки", "Каталог"],
      contextAdvert: ["Яндекс Директ", "Google Adwords"],
    };
  },
};
</script>

<style>
.footer {
  background: #333333;
  padding: 80px 0 25px;
}
.footer__row {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  margin-bottom: 80px;
}
.footer .container {
  max-width: 1180px;
}
.footer-item h5 {
  color: #ffffff;
  text-align: left;
  position: relative;
}
.footer-item h5::after {
  position: absolute;
  content: " ";
  bottom: -30px;
  left: 0;
  width: 34px;
  height: 2px;
  background: #ff0404;
}
.footer-list__item {
  position: relative;
  margin-top: 60px;
  padding-left: 20px;
  color: #ffffff;
}
.footer-list__item:last-child {
  margin-top: 10px;
}
.footer-list__item::before {
  content: "";
  position: absolute;
  left: 0;
  top: 50%;
  transform: translateY(-50%);
  width: 5px;
  height: 5px;
  background-image: url("~@/assets/triangle.svg");
  border-radius: 50%;
}
</style>