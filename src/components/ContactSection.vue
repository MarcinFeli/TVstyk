<template>
	<section id="contact">
		<h1 class="text-h5 text-sm-h4 font-weight-bold text-center mt-3 mb-3 text-uppercase">
			Kontakt
			<div class="outline"></div>
		</h1>
		<div class="contact__bg-img py-5">
			<div class="contact__shadow"></div>
			<v-container class="contact__text">
				<v-row class="text-center align-center" no-gutters>
					<v-col cols="12" sm="4">
						<div>
							<p class="text-h5 font-weight-bold text-uppercase lime--text text--lighten-1">Styk Tower</p>
							<p class="text-body-1">
								ul. Wittiga 8A <br />
								51-628 Wrocław <br />
								(Przy domu akademicki T-19)
							</p>
						</div>
					</v-col>
					<v-col class="mb-5" cols="12" sm="4">
						<div class="contact">
							<p class="text-h5 text-uppercase font-weight-bold lime--text text--lighten-1">Social Media</p>
							<p class="text-body-1 text--white">
								E-mail: <a href="mailto: styk.redakcja@pwr.edu.pl">styk.redakcja@pwr.edu.pl</a>
							</p>
							<a href="https://www.facebook.com/tvs.styk"> <v-icon class="icon" x-large>mdi-facebook</v-icon></a>
							<a href="https://www.instagram.com/telewizjastyk/">
								<v-icon class="icon" x-large>mdi-instagram</v-icon></a
							>
						</div>
					</v-col>
					<v-col cols="12" sm="4">
						<div class="contact">
							<p class="font-weight-bold text-h5 text-uppercase lime--text text--lighten-1">Patroni</p>
							<p class="text-body-1">
								Jesteś zainteresowany patronatem medialnym Telewizji Styk? <br />
								Skontaktuj się z nami aby omówić szczegóły!
							</p>
						</div>
					</v-col>
				</v-row>
			</v-container>
		</div>
	</section>
</template>
<script>
export default {
	name: 'ContactSection',
}
</script>
<style lang="scss">
.contact {
	.icon {
		font-size: 45px;
		padding: 0 5px;
		color: white;
		&:hover {
			color: #0d6efd;
		}
	}
	&__bg-img {
		position: relative;
		padding: 10px 0;
		background-image: url(../assets/img/styk_kontakt.jpg);
		background-size: cover;
		z-index: 0;
	}
	&__shadow {
		position: absolute;
		top: 0;
		height: 100%;
		width: 100%;
		background-color: rgba(0, 0, 0, 0.8);
		z-index: -1;
	}
	&__text {
		color: white;
		z-index: 1;
		h2 {
			text-transform: uppercase;
		}
		a {
			color: #fff;
			text-decoration: none;
			&:hover {
				color: #0d6efd;
			}
		}
	}
}
</style>
