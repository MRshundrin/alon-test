<template>
	<div id="second-footer-wrapper" dir="rtl">
		<div id="navigations-links-wrapper">
			<div id="navigations-links">
				<img src="img/‏‏‏‏‏‏‏‏home/footer/logo-footer.png" alt="logo">
				<ul id="footer-navigations">
					<li><a href="">רושי</a></li>
					<li><a href="">אודות</a></li>
					<li><a href="">פרסומים</a></li>
					<li><a href="">בלוג</a></li>
					<li><a href="">פורום</a></li>
					<li><a href="">הצלחות</a></li>
					<li><a href="">המלצות</a></li>
					<li><a href="">צור קשר</a></li>       
				</ul>
				<div id="social-links">
					<a href="#"><img src="img/‏‏‏‏‏‏‏‏home/footer/youtube_logo.png" alt="logo"></a>
					<a href="#"><img src="img/‏‏‏‏‏‏‏‏home/footer/facebook_logo.png" alt="logo"></a>
				</div>
			</div>
		</div>
		<div id="develop-information" >
			<div>
				<p>2020 ©</p>
				<p dir="rtl">כל הזכויות שמורות</p>
			</div>
			<div>
				<p>בניית אתרים | קידום אתרים</p>
				<img src="img/‏‏‏‏‏‏‏‏home/footer/digotouch_logo.png" alt="logo">
			</div>
		</div>
		<div id="second-footer-contact">
			<div>
				<img src="img/‏‏‏‏‏‏‏‏home/footer/phone_white.png" alt="phone_white">
				<p>זמין 24 שעות ביממה</p>
			</div>
			<div class="mail-white">
				<img src="img/‏‏‏‏‏‏‏‏home/footer/mail_white.png" alt="mail_white">
				<p>ייעוץ ראשוני</p>
			</div>
			<div>
				<img src="img/‏‏‏‏‏‏‏‏home/footer/viber_white.png" alt="viber_white">
				<p>וואטסאפ</p>
			</div>
		</div>
		<a href="#header-wrapper" class="goUP"><img src="img/‏‏‏‏‏‏‏‏home/footer/arrow_top.png" alt="logo"></a>
	</div>
</template>

<style lang="scss">
@import '@/variables.scss';

#second-footer-wrapper {
	width: 100%;
	@include flex(column);
	position: relative;

	#second-footer-contact {
		display: none;
	}

	#navigations-links-wrapper {
		width: 100%;
		height: 100px;
		@include flex(row, center, center);
		background: rgba(243, 246, 248, 0.63);

		#navigations-links {
		width: 1370px;
		@include flex;

			#social-links {
				width: 88px;
				@include flex;
			}
		}

		#footer-navigations {
			width: 934px;
			list-style-type: none;
			@include flex;

			a {
				color: #86939c;
				font-size: 19px;
				line-height: 30px;
			}
		}
	}

	#develop-information {
		width: 1370px;
		padding: 10px 0;
		@include flex;

		div {
			@include flex;
			
			p {
				color: #86939c;
				font-size: 14px;
				font-weight: 400;
			}

			img {
				margin-right: 5px;
			}
		}
	}

	.goUP {
		position: absolute;
		right: 0;
		top: 27px;
	}
}

@media screen and (max-width: 500px) {
  #second-footer-wrapper {

		#navigations-links-wrapper, a {
			display: none;
		}

		#develop-information {
			width: 100%;
			padding: 10px 0;
			@include flex(column, center, center);

			div {
				@include flex;
				
				p {
					color: #86939c;
					font-size: 14px;
					font-weight: 400;
				}

				img {
					margin-right: 5px;
				}
			}
		}

		#second-footer-contact {
			width: 100%;
			height: 53px;
			@include flex(column, center, stretch);
			flex-wrap: wrap;
			background: #007eef;

			div {
				height: 100%;
				width: 33%;
				@include flex(column, center, center);

				p {
					color: #ffffff;
					font-family: $font;
					font-size: 14px;
				}
			}

			.mail-white {
				border-right: #ffffff 1px solid;
				border-left: #ffffff 1px solid;
			}
		}
	} 
}

</style>