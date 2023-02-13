<template>
	<section id="recruitment" class="recruitment">
		<h1 class="text-h4 font-weight-bold text-center mt-3 mb-3 text-uppercase">
			Trwa rekrutacja
			<div class="outline"></div>
		</h1>
		<div class="recruitment__bg-img">
			<div class="recruitment__shadow"></div>
			<div class="container d-flex justify-center">
				<v-col cols="9" class="text-center recruitment__text">
					<p class="font-weight-regular py-3 font-weight-bold text-md-h6 text-sm-subtitle-1 white--text">
						Jesteśmy Telewizją Politechniki Wrocławskiej, do której zapraszamy wszystkich studentów, także z innych
						uczelni. Realizujemy wiele projektów – reportaże, programy publicystyczne, rozrywkowe, informacyjne, live'y
						i wiele więcej. Szkolimy dziennikarzy, operatorów kamer, realizatorów telewizyjnych, montażystów i uczymy
						marketingu. Jesteśmy otwarci na wasze pomysły, kreatywność, aktywność. Wszystkich chętnych zapraszamy do
						współpracy!
					</p>
					<p class="text-md-h4 text-h5">
						<a
							class="recruitment__text"
							href="https://docs.google.com/forms/d/e/1FAIpQLSdVJdZfkrzKV9J3OsvoOlmE6UHDW_dNo5p2OydWiRyJ32dTQQ/closedform"
							target="_blank">
							Formularz kontaktowy
						</a>
					</p>
				</v-col>
			</div>
		</div>
	</section>
</template>
<script>
export default {
	name: 'RecruitmentSection',
}
</script>
<style lang="scss">
.recruitment {
	&__bg-img {
		position: relative;
		background-image: url('../assets/img/header.jpg');
		background-size: cover;
		background-position: center;
		background-attachment: fixed;
	}
	&__shadow {
		position: absolute;
		top: 0;
		height: 100%;
		width: 100%;
		background-color: rgba(0, 0, 0, 0.8);
		z-index: 0;
	}
	&__text {
		z-index: 1;
		a {
			text-decoration: none;
			font-weight: bold;
			text-transform: uppercase;
			transition: scale 0.3s, color 0.3s;
		}
		a:hover {
			transform: scale(1.1);
			color: #cddc39;
		}
	}
}
</style>
