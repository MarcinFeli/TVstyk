<template>
	<v-app>
		<NavigationBar />
		<v-main>
			<HeaderScreen />
			<AboutUsSection />
			<ProgramsSection />
			<AdministrationSection />
			<RecruitmentSection />
			<ContactSection />
			<HelloWorld />
		</v-main>
		<v-footer dark
			><v-col class="text-center" cols="12">
				<strong > &copy; {{ new Date().getFullYear() }} | Telewizja Styk</strong>
			</v-col></v-footer
		>
	</v-app>
</template>

<script>
import NavigationBar from './components/NavigationBar'
import HeaderScreen from './components/HeaderScreen.vue'
import AboutUsSection from './components/AboutUsSection.vue'
import ProgramsSection from './components/ProgramsSection.vue'
import AdministrationSection from './components/AdministrationSection.vue'
import RecruitmentSection from './components/RecruitmentSection.vue'
import ContactSection from './components/ContactSection.vue'

export default {
	name: 'App',

	components: {
		NavigationBar,
		HeaderScreen,
		AboutUsSection,
		ProgramsSection,
		AdministrationSection,
		RecruitmentSection,
		ContactSection,
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
