<template>
  <div class="table__marks">
    <div class="table__mark" v-for="(mark, index) in marks" :key="index">
      <div v-if="mark === true">
        <img :src="markIcon" />
      </div>
      <div v-else>
        <img :src="markGrayIcon" alt="" />
      </div>
    </div>
  </div>
</template>

<script>
import markIcon from "@/assets/mark.svg";
import markGrayIcon from "@/assets/mark-gray.svg";
export default {
  props: ["marks"],
  data() {
    return {
      markIcon,
      markGrayIcon,
    };
  },
};
</script>

<style>
.table__marks {
  width: 50%;
  display: flex;
}
.table__marks{
  width: 25%;
  text-align: center;
  display: flex;
  align-items: center;
}
.table__mark{
  margin-right: 12px;
}
.table__mark div{
  border-right: 2px solid #EAECEF;
  width: 100%;
  padding-right: 62px;
  margin-right: 62px;
}
.table__mark:last-child div{
  border: none;
}
.table__mark div img{
  width: 12px;
  height: 8px;
}
</style>