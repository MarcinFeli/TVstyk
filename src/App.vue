<template>
	<v-app>
		<NavigationBar />
		<v-main>
			<HeaderScreen />
			<AboutUsSection />
			<ProgramsSection />
			<HelloWorld />
		</v-main>
	</v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import NavigationBar from './components/NavigationBar'
import HeaderScreen from './components/HeaderScreen.vue'
import AboutUsSection from './components/AboutUsSection.vue'
import ProgramsSection from './components/ProgramsSection.vue'

export default {
	name: 'App',

	components: {
		HelloWorld,
		NavigationBar,
		HeaderScreen,
		AboutUsSection,
		ProgramsSection,
	},

	data: () => {},
}
</script>

<style lang="scss">
@import './assets/scss/variables.scss';

v-app {
	font-family: $body-font-family !important;
}
.outline {
	text-align: center;
	height: 3px;
	width: 70px;
	margin: 0 auto;
	background-color: cornflowerblue;
}
</style>
