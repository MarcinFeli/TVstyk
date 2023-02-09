<template>
	<v-app>
		<NavigationBar />
		<v-main>
			<HeaderScreen />
			<HelloWorld />
		</v-main>
	</v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import NavigationBar from './components/NavigationBar'
import HeaderScreen from './components/HeaderScreen.vue'

export default {
	name: 'App',

	components: {
		HelloWorld,
		NavigationBar,
		HeaderScreen,
	},

	data: () => {},
}
</script>

<style lang="scss">
*,
*::after,
*::before {
	padding: 0;
	margin: 0;
	box-sizing: border-box;
}
</style>
