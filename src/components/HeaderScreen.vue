<template>
	<div id="header" height="auto" class="header hero-img d-flex justify-center align-center flex-column">
		<div class="hero-shadow"></div>
		<div class="text text-center px-1 d-flex flex-column align-center justify-center">
			<h1 class="white--text text-h3 text-uppercase mb-5">Zapraszamy do naszej ekipy!</h1>
			<p class="white--text text-h5">Trwa rekrutcja!</p>
			<v-btn color="primary">
				<v-icon class="mr-2">mdi-movie-open</v-icon>
				Dołącz do nas!
			</v-btn>
		</div>

		<v-btn @click="scroll" text fab>
			<v-icon color="blue" size="40">mdi-arrow-down</v-icon>
		</v-btn>
	</div>
</template>
<script>
export default {
	name: 'HeaderScreen',

	setup() {
		function scroll() {
			const el = document.getElementById('aboutus')
			el.scrollIntoView({ behavior: 'smooth' })
		}
		return { scroll }
	},
}
</script>
<style lang="scss">
.header {
	scroll-margin: 75px;
}
.hero-img {
	position: relative;
	height: 95vh;
	background-image: url(../assets/img/header.jpg);
	background-size: cover;
	background-position: center;
	background-attachment: fixed;
	z-index: 1;

	.hero-shadow {
		position: absolute;
		height: 100%;
		width: 100%;
		background-color: rgba(0, 0, 0, 0.7);
		z-index: 0;
	}
	.text {
		height: 88%;
		z-index: 2;
	}
}
</style>
