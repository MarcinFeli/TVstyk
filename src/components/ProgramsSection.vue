<template>
	<section id="programs" class="programs">
		<h1 class="text-h5 text-sm-h4  font-weight-bold text-center mt-3 mb-3 text-uppercase">
			Programy
			<div class="outline"></div>
		</h1>
		<div class="programs-box ">
			<v-carousel cycle class="carousel-box" height="auto" hide-delimiters show-arrows="hover">
				<v-carousel-item max-height="600" class="carousel" :src="item.src" v-for="(item, i) in items" :key="i">
					<v-sheet class="sheet" dark color="rgba(0,0,0,0.7)" height="auto">
						<div class="d-flex fill-height flex-column justify-center align-center">
							<v-card-title class="text-sm-h6 text-md-h5 text-lg-h4 text-uppercase font-weight-bold text-center">
								{{ item.title }}</v-card-title
							>
							<v-card-text class="text-center text-subtitle-1">{{ item.text }}</v-card-text>
							
						</div>
					</v-sheet>
				</v-carousel-item>
			</v-carousel>
		</div>
	</section>
</template>
<script>
export default {
	name: 'ProgramsSection',
	data() {
		return {
			items: [
				{
					src: 'https://styk-telewizja.netlify.app/img/styk_spotlight.jpg',
					title: 'Spotlight',
					text: 'Program, w którym w kilka minut wyjaśniamy fascynujące aspekty otaczającego nas świata.',
				},
				{
					src: 'https://styk-telewizja.netlify.app/img/styk_rzeczywi%C5%9Bcie.jpg',
					title: 'Rzeczywiście',
					text: 'Prowadzimy wywiady z różnymi bardzo ciekawymi i inspirującymi ludźmi.',
				},
				{
					src: 'https://styk-telewizja.netlify.app/img/styk_wymiar.jpg',
					title: 'Świat na wymiar',
					text: 'Jest to program, w którym podsumowujemy najważniejsze wydarzenia miesiąca',
				},
				{
					src: 'https://styk-telewizja.netlify.app/img/styk_kino.jpg',
					title: 'Kino na weekend',
					text: 'Szukasz dobergo filmu? A może chcesz się zrelaksować przy dobrym filmie? Obczaj nasz program Kino na Weekend gdzie polecamy różne nowości!',
				},
				{
					src: 'https://styk-telewizja.netlify.app/img/styk_inne.jpg',
					title: 'Spotlight',
					text: 'Sprawdź wszystkie programy i aktualności na naszym Facebooku',
				},
			],
		}
	},
}
</script>
<style lang="scss">

.programs {
	scroll-margin: 69px;
}
.carousel {
	position: relative;
	.sheet {
		position: absolute;
		bottom: 0;
		right: 0;
		left: 0;
	}
}
.text-h2 {
	background-position: center;
	background-size: cover;
}

@media (min-width: 600px) {
	.programs-box {
		width: 60%;
		margin: 0 auto;
	}
}
@media (min-width: 800px) {
	.programs-box {
		width: 70%;
		margin: 0 auto;
	}
}
</style>
