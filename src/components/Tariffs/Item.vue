<template>
  <div class="tariffs-item">
    <TagH type="h5">Продвижение по позициям</TagH>
    <img :src="tariffImg" />
    <div class="tariffs-item__description">
      Продвинем 10 сылок на первые места
    </div>
    <span class="tariffs-item__price">15000 руб</span>
    <Button text="Оставить заявку" className="btn-light" />
  </div>
</template>

<script>
import TagH from "@/components/TagH/TagH.vue";
import tariffImg from "@/assets/tariffs-item-1.png";
import Button from "@/components/Buttons/Button.vue";
export default {
  components: { TagH, Button },
  data() {
    return {
      tariffImg,
    };
  },
};
</script>

<style>
</style>