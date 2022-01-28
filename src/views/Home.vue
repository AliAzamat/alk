<template>
  <main>
    <section class="hero">
      <img class="hero__img" :src="heroImg" alt="Our Work Routine" />
      <div>
        <TagH className="hero__title" type="h1"> Продвижение сайтов </TagH>
      </div>
    </section>
    <Calculator />
    <Rates />
    <ApplyForm />
    <Reviews />
    <Tariffs />
    <Portfolio />
    <Footer />
  </main>
</template>

<script>
import Calculator from "@/components/Calculator/Calculator.vue";
import Rates from "@/components/Rates/Rates.vue";
import heroImg from "@/assets/hero.jpg";
import ApplyForm from "@/components/ApplyForm/ApplyForm.vue";
import Reviews from "@/components/Reviews/Reviews.vue";
import Tariffs from "@/components/Tariffs/Tariffs.vue";
import Portfolio from "@/components/Portfolio/Portfolio.vue";
import Footer from "@/components/Footer/Footer.vue";
export default {
  components: {
    Calculator,
    Rates,
    ApplyForm,
    Reviews,
    Tariffs,
    Portfolio,
    Footer,
  },
  data() {
    return {
      heroImg,
    };
  },
};
</script>

<style>
main {
  height: 500vh;
}
.hero {
  text-align: center;
}
.hero__img {
  min-height: 358px;
  max-height: 558px;
  min-width: 100%;
  max-width: 100%;
  margin-bottom: 80px;
}
.hero div {
  margin-bottom: 45px;
}
.hero__title {
  font-size: 55px;
  font-family: "Fira Sans Extra Condensed";
  font-style: normal;
  line-height: 100%;
  text-transform: uppercase;
  color: #333333;
  text-align: center;
  font-weight: 700;
  text-align: center;
}
</style>