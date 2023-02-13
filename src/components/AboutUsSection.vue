<template>
	<section id="aboutus" class="about-us">
		<h1 class="text-h4 font-weight-bold text-center mt-3 mb-3 text-uppercase">
			Kim jesteśmy?
			<div class="outline"></div>
		</h1>
		<div height="auto" class="about-us__img">
			<div class="about-us__shadow"></div>
			<div class="about-us__text white--text">
				<p class="text-center font-weight-bold body-1">
					Zespół Telewizji Studenckiej Politechniki Wrocławskiej STYK tworzą studenci różnych uczelni. Łączy nas wspólna
					idea tworzenia jedynego takiego medium, gdzie możemy razem się rozwijać. Nasza siedziba to mały Stykowy
					budynek przy ul. Wittiga 8A. Jesteśmy otwarci na Wasze pomysły, kreatywność i aktywność. Wszystkich chętnych
					zapraszamy do współpracy! To doskonała okazja, aby zobaczyć jak powstają nagrania, na czym polega montaż oraz
					nauczyć się obsługi kamery 💁‍♀️🎬
				</p>
				<iframe
					class="about-us__video"
					src="https://www.youtube.com/embed/0JNxEFS2oCc?feature=oembed"
					title="YouTube video"
					allowfullscreen></iframe>
			</div>
		</div>
	</section>
</template>
<script>
export default {
	name: 'AboutUsSection',
}
</script>
<style lang="scss">
@import '../assets/scss/variables.scss';
.about-us {
	scroll-margin: 75px;
	&__img {
		position: relative;
		display: flex;
		justify-content: center;
		background-image: url(../assets/img/aboutUs.jpg);
		background-position: center;
		background-size: cover;
		z-index: 1;
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
		display: flex;
		padding: 20px 10px;
		flex-direction: column;
		align-items: center;
		width: 75%;
		z-index: 2;
	}
	&__video {
		height: 60vh;
		width: 100%;
	}
}
</style>
