<template>
	<div class="analysis">
		<TagH className="analysis__title" type="h3"> Глубокий анализ </TagH>
		<div class="test">
			<div class="analysis__row">
				<div class="analysis__item">
					<TagH className="analysis__subtitle" type="h5">
						Глубокий анализ
					</TagH>
					<p>SEO, юзабилити, тексты. Пример аудита</p>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
import TagH from "@/components/TagH/TagH.vue";
export default {
	components: { TagH },
};
</script>

<style>
.analysis__title {
	padding: 8px 0;
	border-radius: 5px;
	background: linear-gradient(0deg, #ffd773, #ffd773), #f4f7fe;
}
.analysis__row {
	display: flex;
	border-bottom: 1px solid red;
}
.analysis__subtitle {
	text-align: left;
	margin-bottom: 10px;
}
.analysis__item {
	padding-bottom: 20px;
}
.test {
  padding: 35px 0;
}
</style>