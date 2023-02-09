<template>
	<nav>
		<v-app-bar color="dark" dark>
			<v-app-bar-nav-icon class="hidden-lg-and-up" @click="drawer = !drawer"></v-app-bar-nav-icon>
			<v-btn target="_blank" text x-large>
				<v-img
					alt="Vuetify Logo"
					class="shrink mr-2"
					contain
					src="../assets/cropped-ikona.png"
					transition="scale-transition"
					width="40" />
				Telewizja <span class="lime--text text--lighter-2"> S</span
				><span class="light-blue--text text--lighten-1"> T</span><span class="lime--text text--lighter-2"> Y</span
				><span class="light-blue--text text--lighten-1"> K</span>
			</v-btn>
			<v-spacer></v-spacer>
			<v-hover v-slot="{ hover }">
				<v-btn
					href="https://github.com/vuetifyjs/vuetify/releases/latest"
					target="_blank"
					text
					:color="hover ? 'blue' : 'white'">
					Strona główna
				</v-btn>
			</v-hover>
			<v-hover v-slot="{ hover }">
				<v-btn
					href="https://github.com/vuetifyjs/vuetify/releases/latest"
					target="_blank"
					text
					:color="hover ? 'blue' : 'white'">
					O nas
				</v-btn>
			</v-hover>
			<v-hover v-slot="{ hover }">
				<v-btn
					href="https://github.com/vuetifyjs/vuetify/releases/latest"
					target="_blank"
					text
					:color="hover ? 'blue' : 'white'">
					Programy
				</v-btn>
			</v-hover>
			<v-hover v-slot="{ hover }">
				<v-btn
					href="https://github.com/vuetifyjs/vuetify/releases/latest"
					target="_blank"
					text
					:color="hover ? 'blue' : 'white'">
					Zarząd
				</v-btn>
			</v-hover>
			<v-hover v-slot="{ hover }">
				<v-btn
					href="https://github.com/vuetifyjs/vuetify/releases/latest"
					target="_blank"
					text
					:color="hover ? 'blue' : 'white'">
					Rekrutacja
				</v-btn>
			</v-hover>
			<v-hover v-slot="{ hover }">
				<v-btn
					href="https://github.com/vuetifyjs/vuetify/releases/latest"
					target="_blank"
					text
					:color="hover ? 'blue' : 'white'">
					Kontakt
				</v-btn>
			</v-hover>
		</v-app-bar>

		<v-navigation-drawer class="hidden-lg-and-up" app v-model="drawer" absolute temporary>
			<v-list nav dense>
				<v-list-item-group v-model="group" active-class="deep-purple--text text--accent-4">
					<v-list-item>
						<v-list-item-icon>
							<v-icon>mdi-home</v-icon>
						</v-list-item-icon>
						<v-list-item-title>Strona główna</v-list-item-title>
					</v-list-item>
					<v-list-item>
						<v-list-item-icon>
							<v-icon>mdi-account</v-icon>
						</v-list-item-icon>
						<v-list-item-title>O nas</v-list-item-title>
					</v-list-item>
					<v-list-item>
						<v-list-item-icon>
							<v-icon>mdi-projector-screen</v-icon>
						</v-list-item-icon>
						<v-list-item-title>Programy</v-list-item-title>
					</v-list-item>
					<v-list-item>
						<v-list-item-icon>
							<v-icon>mdi-account</v-icon>
						</v-list-item-icon>
						<v-list-item-title>Zarząd</v-list-item-title>
					</v-list-item>
					<v-list-item>
						<v-list-item-icon>
							<v-icon>mdi-account-group</v-icon>
						</v-list-item-icon>
						<v-list-item-title>Rekrutacja</v-list-item-title>
					</v-list-item>
					<v-list-item>
						<v-list-item-icon>
							<v-icon>mdi-phone</v-icon>
						</v-list-item-icon>
						<v-list-item-title>Kontakt</v-list-item-title>
					</v-list-item>
				</v-list-item-group>
			</v-list>
		</v-navigation-drawer>
	</nav>
</template>
<script>
export default {
	name: 'NavigationBar',

	data() {
		return {
			drawer: false,
		}
	},
}
</script>
<style lang=""></style>
