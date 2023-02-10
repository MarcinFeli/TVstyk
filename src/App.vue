<template>
	<v-app>
		<NavigationBar />
		<v-main>
			<HeaderScreen />
			<AboutUsSection />
			<HelloWorld />
		</v-main>
	</v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import NavigationBar from './components/NavigationBar'
import HeaderScreen from './components/HeaderScreen.vue'
import AboutUsSection from './components/AboutUsSection.vue'

export default {
	name: 'App',

	components: {
		HelloWorld,
		NavigationBar,
		HeaderScreen,
		AboutUsSection,
	},

	data: () => {},
}
</script>

<style lang="scss">
@import './assets/scss/variables.scss';

v-app {
	font-family: $body-font-family !important;
}
</style>
