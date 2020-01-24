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
			<div>
				<img src="img/‏‏‏‏‏‏‏‏home/footer/mail.png" alt="mail">
				<p class="contact">דואר אלקטרוני</p>
				<p class="type-of-contact">office@alonerez.co.il</p>
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


</style>