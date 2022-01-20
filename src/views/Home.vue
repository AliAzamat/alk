<template>
	<main>
		<section class="hero">
			<img class="hero__img" :src="heroImg" alt="Our Work Routine" />
			<TagH className="hero__title" type="h1"> Продвижение сайтов </TagH>
		</section>
    <Calculator />
	</main>
</template>

<script>
import TagH from "@/components/TagH/TagH.vue";
import Calculator from '@/components/Calculator/Calculator.vue'
import heroImg from "@/assets/hero.jpg";
export default {
	components: { TagH,Calculator },
	data() {
		return {
			heroImg,
		};
	},
};
</script>

<style>
.hero__img {
	min-height: 358px;
	max-height: 558px;
}
.hero__title {
	margin: 80px 0 45px;
}
</style>