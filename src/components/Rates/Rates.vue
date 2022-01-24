<template>
	<section class="rates">
		<div class="container">
			<TagH type="h2"> Сравнение тарифов </TagH>
			<div class="rates__titles">
				<span>Продвинутый</span>
				<span>Комплексный</span>
				<span>Оптимизация</span>
				<span>Потрясающий</span>
			</div>
			<Analysis />
			<TagH className="rates__blue" type="h3">
				Работа с ключевыми словами
			</TagH>
		</div>
	</section>
</template>

<script>
import TagH from "@/components/TagH/TagH.vue";
import Analysis from "./Analysis.vue";
export default {
	components: { TagH, Analysis },
};
</script>

<style>
.rates__titles {
	text-align: right;
	margin-bottom: 20px;
}
.rates h2{
	margin-bottom: 45px;
}
.rates__blue,
.rates__yellow {
	padding: 8px 0;
	border-radius: 5px;
}
.rates__blue {
	background: linear-gradient(0deg, #77cbfa, #77cbfa), #f4f7fe;
}
.rates__yellow {
	background: linear-gradient(0deg, #ffd773, #ffd773), #f4f7fe;
}
.rates .rates__titles span {
	margin-left: 40px;
	font-family: Fira Sans Extra Condensed;
	font-style: normal;
	font-weight: 600;
	font-size: 16px;
	line-height: 150%;
	text-transform: uppercase;
	color: #333333;
}
</style>