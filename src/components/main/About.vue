<template>
	<div id="about-section">
		<h2>אודות</h2>
		<div id="about-section-content">
			<div id="about-section-content-left" dir="rtl">
				<h3>כבר יותר מ-10 שנים שאני מייצג בהצלחה רבה מאות לקוחות מרוצים.</h3>
				<p>במשך למעלה מ-10 שנים אני מייצג בהצלחה רבה לקוחות מכל שכבות האוכלוסייה, בהליכים פליליים וצבאיים.</p>
				<p>בזכות הניסיון המעשי הרב שצברתי בניהול תיקים מגוונים בבתי המשפט ולאחר ייצוג של מאות לקוחות בהליכים משפטיים רבים, אני יכול להעיד על עצמי, במלוא הכנות והצניעות, שאני הכתובת המשפטית הטובה ביותר עבורך.</p>
				<a href="">קרא עוד <i class="fas fa-chevron-left"></i></a>
			</div>
			<div id="about-section-content-right">
				<button><i class="fas fa-play"></i></button>
			</div>
		</div>
	</div>
</template>

<style lang="scss">
@import '@/variables.scss';

#about-section {
	@include flex(column);
	margin-top: 70px;
	margin-bottom: 82px;

	h2 {
		color: $main-color;
		font-family: $font-bold;
		font-size: 48px;
	}

	&-content {
		width: 1369px;
		height: 385px;
		box-shadow: 0 8px 84px rgba(83, 103, 118, 0.13);
		background-color: #ffffff;

		@include flex(row, center, stretch);

		div {
			width: 50%;
		}

		&-left {
			@include flex(column, flex-start, flex-start);
			padding-right: 50px;
			box-sizing: border-box;

			h3 {
				color: $main-color;
				font-family: $font;
				font-weight: 300;
				font-size: 36px;
			}

			p {
				color: $text-color;
				font-family: $font;
				font-size: 18px;
				line-height: 28px;
			}

			a {
				color: $text-color;
				font-family: $font-bold;
				font-size: 18px;
				line-height: 28px;

				i {
					font-size: 9px;
					color: #007eef;
				}
			}
		}

		&-right {
			background: url(../../../public/img/‏‏‏‏‏‏‏‏home/04/video.jpg);
			background-size: cover;
			background-repeat: no-repeat;
			@include flex(row, center, center);

			button {
				width: 62px;
				height: 62px;
				border: 1px solid rgba(255, 255, 255, 0.6);;
				background-color: rgba(0, 0, 0, 0.2);
				text-shadow: white 1px 1px 0, white -1px -1px 0, white -1px 1px 0, white 1px -1px 0;
				font-size: 20px;
				color: #007eef;
				padding: 20px;
				box-sizing: border-box;
			}
		}
	}
}

@media screen and (max-width: 500px) {
	#about-section {
		margin-top: 60px;
		margin-bottom: 60px;

		h2 {
			font-size: 36px;
		}

		&-content {
			width: 344px;
			height: 561px;
		
			@include flex(column, center, stretch);

			div {
				width: 100%;
			}

			&-left {
				padding: 0 25px 30px 0;
				box-sizing: border-box;

				h3 {
					font-size: 22px;
				}

				p {
					width: 300px;
				}
			}

			&-right {
				height: 198px;
			}
		}
	}
}
</style>