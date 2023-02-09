<template>
	<v-app>
    <NavigationBar />
    <v-main>
			<HelloWorld />
		</v-main>
	</v-app>
</template>

<script>
import HelloWorld from './components/HelloWorld'
import NavigationBar from './components/NavigationBar'

export default {
	name: 'App',

	components: {
		HelloWorld,
		NavigationBar,
	},

	data: () => {},
}
</script>

<style lang="scss"></style>
