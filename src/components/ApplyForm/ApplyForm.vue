<template>
  <section class="apply-form">
    <div class="container">
      <TagH className="apply-form__title" type="h2">Форма заявки</TagH>
      <form class="apply-form__form">
        <div class="apply-form__left">
          <div>
            <Input/>
            <Input/>
          </div>
          <div>
            <Input/>
            <Input/>
          </div>
        </div>
        <div>
          <Checkbox
            class="apply-form__checkbox"
            name="apply-form"
            label="Нажимая на кнопку, вы соглашаетесь с нашей политикой обработки"
          />
          <Button className="btn-primary" text="Оставить заявку" />
        </div>
      </form>
    </div>
  </section>
</template>

<script>
import TagH from "@/components/TagH/TagH.vue";
import Button from "@/components/Buttons/Button.vue";
import Checkbox from "@/components/Inputs/Checkbox";
import Input from "@/components/Inputs/Input";
export default {
  components: { TagH, Button, Checkbox, Input },
};
</script>

<style>
.apply-form__left{
  padding-right: 20px;
}
.apply-form__left div{
  display: flex;
}
input{
  margin-bottom: 20px;
  margin-right: 20px;
  width: 314px;
  color: #ffffff;
}
input:last-child{
  margin-right: 0;
}
.apply-form {
  background: #333333;
  padding: 80px 0;
}
.apply-form__form{
  display: flex;
}
.apply-form__form button{
  width: 100%;
}
.apply-form__title{
  margin-bottom: 45px;
}
.apply-form__title,
.apply-form .apply-form__checkbox span {
  color: #fff;
}
.apply-form .apply-form__checkbox span {
  font-weight: 500;
  font-size: 14px;
}
.apply-form .apply-form__checkbox {
  display: flex;
  margin-bottom: 28px;
}
.apply-form .apply-form__checkbox label::before{
  top: 50%;
  transform: translateY(-50%);
}
</style>