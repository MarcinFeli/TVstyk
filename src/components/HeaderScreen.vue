<template>
	<div class="hero-img d-flex justify-center">
		<div class="hero-shadow"></div>
		<div class="text d-flex flex-column align-center justify-center">
			<h1 class="center">Zapraszamy do naszej ekipy!</h1>
			<p>Trwa rekrutcja!</p>
		</div>
	</div>
</template>
<script>
export default {
	name: 'HeaderScreen',
}
</script>
<style lang="scss">
.hero-img {
	position: relative;
	height: 100vh;
	background-image: url(../assets/mountains-1412683_1280.png);
	background-size: cover;
	background-position: center;
	background-attachment: fixed;

	.hero-shadow {
		position: absolute;
		height: 100%;
		width: 100%;
		background-color: rgba(0, 0, 0, 0.7);
	}
}
</style>
