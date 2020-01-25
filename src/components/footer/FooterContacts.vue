<template>
	<div id="footer-contact-wrapper">
		<div id="footer-contact">
			<div>
				<img src="img/‏‏‏‏‏‏‏‏home/footer/location.png" alt="location">
				<p class="contact">כתובתנו</p>
				<p class="type-of-contact">שאול המלך 8 תל-אביב</p>
			</div>
			<div>
				<img src="img/‏‏‏‏‏‏‏‏home/footer/phone.png" alt="phone">
				<p class="contact">03-6520155</p>
				<p class="type-of-contact">טלפון במשרד</p>
			</div>
			<div>
				<img src="img/‏‏‏‏‏‏‏‏home/footer/whats_app.png" alt="whats_app">
				<p class="contact">050-7368203</p>
				<p class="type-of-contact">נייד</p>
			</div>
			<div>
				<img src="img/‏‏‏‏‏‏‏‏home/footer/fax.png" alt="fax">
				<p class="contact">03-6495510</p>
				<p class="type-of-contact">פקס</p>
			</div>
			<div id="contact-mail">
				<img src="img/‏‏‏‏‏‏‏‏home/footer/mail.png" alt="mail">
				<p class="contact">דואר אלקטרוני</p>
				<p class="type-of-contact">office@alonerez.co.il</p>
			</div>
		</div>
		<div id="footer-contact-mobile">
			<div id="contact-mail">
				<img src="img/‏‏‏‏‏‏‏‏home/footer/mail.png" alt="mail">
				<div>
					<p class="contact">דואר אלקטרוני</p>
					<p class="type-of-contact">office@alonerez.co.il</p>
				</div>
			</div>
			<div class="social-links">
				<a href="#"><img src="img/‏‏‏‏‏‏‏‏home/footer/youtube_logo.png" alt="logo"></a>
				<a href="#"><img src="img/‏‏‏‏‏‏‏‏home/footer/facebook_logo.png" alt="logo"></a>
			</div>
		</div>
	</div>
</template>

<style lang="scss">
@import '@/variables.scss';

#footer-contact-wrapper {
	width: 100%;
	border-bottom: 1px solid #b9b9b9;
}

#footer-contact-mobile {
	display: none;
}

#footer-contact {
	width: 1244px;
	@include flex;
	margin: 40px auto;

	div {
		@include flex(column);
		height: 98px;

		.contact {
			color: #1c1d21;
			font-family: $font-bold;
			font-size: 22px;
			font-weight: 400;
			line-height: 26px;
		}

		.type-of-contact {
			color: #1c1d21;
			font-family: $font;
			font-size: 16px;
			font-weight: 400;
			line-height: 26px;
		}
	}
}

@media screen and (max-width: 500px) {
	#footer-contact-mobile {
		width: 100%;
		height: 86px;
		@include flex(row, space-around);
		background-color: #f7f9fb;

		.social-links {
			width: 88px;
			@include flex;
		}

		#contact-mail {
			@include flex(row, center, center);
			height: 100%;
			width: 50%;

			div {
				@include flex(column, center, center);
				padding-right: 10px;

				.contact {
					color: #1c1d21;
					font-family: $font-bold;
					font-size: 22px;
					font-weight: 400;
					line-height: 15px;
				}

				.type-of-contact {
					color: #1c1d21;
					font-family: $font;
					font-size: 16px;
					font-weight: 400;
					line-height: 15px;
				}
			}
		}
	}


	#footer-contact-wrapper {
		width: 100%;
		border-bottom: 1px solid #b9b9b9;
	}

	#footer-contact {
		width: 100%;
		border-bottom: 1px solid #b9b9b9;
		@include flex(row, center);
		flex-wrap: wrap;
		margin: 0;

		#contact-mail {
			display: none;
		} 

		div {
			@include flex(column, center);
			height: 130px;
			width: 187px;
		}
	}
}
</style>