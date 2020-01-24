<template>
	<div id="black-banner" dir="rtl">
		<div id="information-wrapper" dir="ltr">
			<h2>התמחות בכל סוגי העבירות הפליליות</h2>
			<p>חוק העונשין של מדינת ישראל מאגד תחתיו סוגים שונים של עבירות פליליות. משרד עורכי דין פליליים תל אביב אלון ארז מתמחה בייצוג חשודים ונאשמים בעבירות אלו במלוא המסירות.</p>
			<p>בשל האמונה כי כל אדם זכאי לייצוג ללא אבחנה, עו"ד פלילי אלון ארז פועל למיצוי זכויותיהם של חשודים ונאשמים בדרכים רבות החל בייצוג בהליכי מעצר ושימוע לפני הגשת כתב האישום, עובר בייצוג בהליכים משפטיים בבית המשפט כולל ניהול הוכחות וחקירות עדים וכלה בהגשת ערעורים, כתיבת בקשות חנינה לנשיא המדינה וייצוג אסירים בפני וועדת השחרורים וועדות השב"ס.</p>
			<p>בנוסף, עורך דין פלילי בתל אביב אלון ארז משתף פעולה עם גורמים מקצועיים רבים לרבות חוקרים פרטיים, מומחים בתחום הנשק, ואנשי מקצוע מתחומי הפסיכולוגיה, הפתולוגיה והרווחה.</p>
			<p>חוק העונשין של מדינת ישראל מאגד תחתיו סוגים שונים של עבירות פליליות. משרד עורכי דין פליליים תל אביב אלון ארז מתמחה בייצוג חשודים ונאשמים בעבירות אלו במלוא המסירות.</p>
			<p>בשל האמונה כי כל אדם זכאי לייצוג ללא אבחנה, עו"ד פלילי אלון ארז פועל למיצוי זכויותיהם של חשודים ונאשמים בדרכים רבות החל בייצוג בהליכי מעצר ושימוע לפני הגשת כתב האישום, עובר בייצוג בהליכים משפטיים בבית המשפט כולל ניהול הוכחות וחקירות עדים וכלה בהגשת ערעורים, כתיבת בקשות חנינה לנשיא המדינה וייצוג אסירים בפני וועדת השחרורים וועדות השב"ס.</p>
			<p>בנוסף, עורך דין פלילי בתל אביב אלון ארז משתף פעולה עם גורמים מקצועיים רבים לרבות חוקרים פרטיים, מומחים בתחום הנשק, ואנשי מקצוע מתחומי הפסיכולוגיה, הפתולוגיה והרווחה.</p>
		</div>
		<div id="work-directions-wrapper">
			<div id="work-directions-content">
				<button @click="refresh"><i class="fas fa-chevron-right"></i></button>
				<div class="work-directions">
						<div class="work-directions-card" v-if="counter == 1">
							<h4>עבירות מין</h4>
							<p>עבירות מין מאגדות תחתן קשת רחבה של מקרים והן נחשבות לתחום משפטי מורכב הדורש בקיאות והיכרות עם החוק והפסי</p>
							<a href="">קרא עוד <i class="fas fa-chevron-left"></i></a>
						</div>
						<div class="work-directions-card" v-if="counter == 1">
							<h4>עבירות סמים</h4>
							<p>משרד עו"ד אלון ארז מתמחה בייצוג חשודים ונאשמים בעבירות סמים על סוגיהן השונים, החל מסחר וייבוא ועד להחזקה. </p>
							<a href="">קרא עוד <i class="fas fa-chevron-left"></i></a>
						</div>
						<div class="work-directions-card" v-if="counter == 1">
							<h4>הטרדה מינית</h4>
							<p>אם אתם חשודים בהטרדה מינית אתם זקוקים לייעוץ עו"ד מקצועי בתחום הפלילי שילווה וייצג אתכם הן במהלך חקירות </p>
							<a href="">קרא עוד <i class="fas fa-chevron-left"></i></a>
						</div>
						<div class="work-directions-card" v-if="counter == 1">
							<h4>רצח</h4>
							<p>עבירת רצח היא אחת החמורות ביותר בתחום המשפט הפלילי ולכן יש לשכור את שירותיו של עורך דין פלילי בתל אביב, עו"ד </p>
							<a href="">קרא עוד <i class="fas fa-chevron-left"></i></a>
						</div>
						<div class="work-directions-card" v-if="counter == 2">
							<h4>עבירות סמים</h4>
							<p>משרד עו"ד אלון ארז מתמחה בייצוג חשודים ונאשמים בעבירות סמים על סוגיהן השונים, החל מסחר וייבוא ועד להחזקה. </p>
							<a href="">קרא עוד <i class="fas fa-chevron-left"></i></a>
						</div>
						<div class="work-directions-card" v-if="counter == 2">
							<h4>עבירות מין</h4>
							<p>עבירות מין מאגדות תחתן קשת רחבה של מקרים והן נחשבות לתחום משפטי מורכב הדורש בקיאות והיכרות עם החוק והפסי</p>
							<a href="">קרא עוד <i class="fas fa-chevron-left"></i></a>
						</div>
						<div class="work-directions-card" v-if="counter == 2">
							<h4>רצח</h4>
							<p>עבירת רצח היא אחת החמורות ביותר בתחום המשפט הפלילי ולכן יש לשכור את שירותיו של עורך דין פלילי בתל אביב, עו"ד </p>
							<a href="">קרא עוד <i class="fas fa-chevron-left"></i></a>
						</div>
						<div class="work-directions-card" v-if="counter == 2">
							<h4>הטרדה מינית</h4>
							<p>אם אתם חשודים בהטרדה מינית אתם זקוקים לייעוץ עו"ד מקצועי בתחום הפלילי שילווה וייצג אתכם הן במהלך חקירות </p>
							<a href="">קרא עוד <i class="fas fa-chevron-left"></i></a>
						</div>
				</div>
				<div class="work-directions-mobile">
					<div class="work-directions-card" v-if="counter == 1">
							<h4>עבירות מין</h4>
							<p>עבירות מין מאגדות תחתן קשת רחבה של מקרים והן נחשבות לתחום משפטי מורכב הדורש בקיאות והיכרות עם החוק והפסי</p>
							<a href="">קרא עוד <i class="fas fa-chevron-left"></i></a>
						</div>
						<div class="work-directions-card" v-if="counter == 2">
							<h4>עבירות סמים</h4>
							<p>משרד עו"ד אלון ארז מתמחה בייצוג חשודים ונאשמים בעבירות סמים על סוגיהן השונים, החל מסחר וייבוא ועד להחזקה. </p>
							<a href="">קרא עוד <i class="fas fa-chevron-left"></i></a>
						</div>
				</div>
				<button @click="refresh"><i class="fas fa-chevron-left"></i></button>
			</div>
			<div class="dot-section">
				<div class="dot" :class="{ active: counter == 1 }"></div>
				<div class="dot" :class="{ active: counter == 2 }"></div>
			</div>
		</div>
	</div>
</template>

<script>

	export default {
		name: 'blackBanner',
		data: () => ({
			counter: 1
		}),
		methods: {
			refresh () {
				if (this.counter == 1) {
          this.counter = 2
        } else {
          this.counter = 1
        }
			}
		}
	}
</script>

<style lang="scss">
@import '@/variables.scss';

#black-banner {
	width: 100%;
	height: 675px;
	background: url(../../../public/img/‏‏‏‏‏‏‏‏home/05/criminal_bg.jpg);
	background-size: contain;
	background-repeat: no-repeat;
	background-position: left;
	background-color: black;
	color: $light-color;
	padding: 80px 14%;
	box-sizing: border-box;
	position: relative;

	#information-wrapper {
		width: 540px;
		height: 444px;
		overflow: auto;
		text-align: right;
		padding-right: 26px;
	

      &::-webkit-scrollbar {
        width: 1px;
      }
      &::-webkit-scrollbar-track-piece {
				background-color: rgba(255, 255, 255, 0.22);
      }
      &::-webkit-scrollbar-thumb {
				background-color: white;
      }
	}

	h2 {
		font-family: $font-bold;
		font-size: 48px;
		line-height: 48px;
	}
	
	p {
		font-family: $font;
		font-size: 18px;
		margin-top: 10px;
		line-height: 28px;
		font-weight: 100;
	}
}

#work-directions-wrapper {
	height: 220px;
	@include flex(column);
	position: absolute;
	left: 50%;
  transform: translate(-50%);
	bottom: -140px;
	z-index: 1;

	#work-directions-content {
		width: 1510px;
		@include flex;
	}

	.work-directions-mobile {
		display: none;
	}

	.work-directions {
		width: 1372px;
		@include flex;

		&-card {
			width: 320px;
			height: 159px;
			background: $light-color;
			@include flex(column, flex-start, flex-start);
			padding: 25px 30px 0 0;
			box-sizing: border-box;
			position: relative;
			box-shadow: 0 8px 166px rgba(83, 103, 118, 0.33);

			h4 {
				color: #2b2c32;
				font-family: $font-bold;
				font-size: 26px;
				line-height: 28px;
				border-bottom: 3px solid #007eef;
				margin: 0;
			}

			p {
				color: $second-color;
				font-family: $font;
				font-size: 17px;
				line-height: 20px;
				font-weight: 300;
			}

			a {
				display: none;
				position: absolute;
				bottom: 30px;
				color: #2b2c32;
				font-family: $font-bold;
				font-size: 19px;
				font-weight: 400;
				line-height: 30px;
				z-index: 1;

				i {
					font-size: 9px;
					color: #007eef;
				}
			}

			&:after {
				position: absolute;
				bottom: 0;  
				left: 0;
				height: 100%;
				width: 100%;
				content: "";
				background-image: linear-gradient(to top, #ffffff 0%, rgba(255, 255, 255, 0) 100%);
			}

			&:hover a {
				display: block;
			}
		}	
	}
	
	button {
    border: none;
    width: 46px;
    height: 46px;
    background-color: #007eef;
    color: #dee7ed;
    font-weight: 100;
    font-size: 20px;
	}
	.dot-section {
		@include flex;
		width: 41px;

		.dot {
			width: 9px;
			height: 9px;
			background-color: #dee7ed;
		}
		
		.active {
			background-color: #007eef;
		}
	}
}

@media screen and (max-width: 500px) {
  #black-banner {
		height: 606px;
		background: url(../../../public/img/‏‏‏‏‏‏‏‏home/05/criminal_bg_mobile.png);
		background-size: cover;
		background-position: -135px;
		padding: 50px 7%;
		
		

		#information-wrapper {
			width: 100%;
			height: 450px;
			padding-right: 17px;
		}

		h2 {
			font-size: 36px;
			line-height: 36px;
		}
		
		p {
			font-size: 16px;
			line-height: 22px;
		}
	}

	#work-directions-wrapper {
		height: 187px;
		bottom: -117px;
		z-index: 1;

		#work-directions-content {
			width: 377px;
			@include flex;
		}

		.work-directions-mobile {
			@include flex;
			width: 285px;
			height: 140px;

			.work-directions-card {
				width: 100%;
				height: 100%;
				padding: 25px 18px 0 0;

				p {
					width: 260px;
				}
			}
		}
		
		.work-directions {
			display: none;	
		}
		
		button {
			width: 36px;
		}
	}
}

</style>