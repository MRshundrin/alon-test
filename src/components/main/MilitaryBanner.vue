<template>
	<div id="military-banner">
		<div id="information-wrapper" dir="ltr">
			<h2>עו"ד פלילי אלון ארז –ייצוג נאשמים במשפט הצבאי</h2>
			<p class="subtitle">להביא את הלקוח למקום הטוב ביותר האפשרי מבחינת נתוני התיק.</p>
			<p>קיימים לא מעט עורכי דין פליליים בתל אביב, אשר בטוחים שביכולתם להעניק ייעוץ וייצוג מקצועי מול המערכת הצבאית, אך בפועל לא מן הנמנע כי גם העורך הדין הנחשב ביותר בשוק לא יידע לייצג נאשמים כהלכה בתחום המשפט הצבאי.</p>
			<p>זאת, משום שהמערכת הצבאית והפרקליטות הצבאית שונות בתכלית ממקבילותיהן האזרחיות. בנוסף, דיני עבירות פליליות בצבא שונים לחלוטין מאלו אשר נידונים בבתי משפט "אזרחיים".</p>
			<p>עורך דין פלילי במרכז המתמחה בתחום הצבאי, וזהו תחום התמחות המרכזי עבורו, יידע לספק מעטפת של סיוע וטיפול מקצועי בערכאות הצבאיות בייצוג במגוון עבירות, החל משימוש בנשק באופן בלתי חוקי, עריקות, סחר באמל"ח, ועד לעבירות כמו עישון סמים, נפקדות ועוד.</p>
			<p>קיימים לא מעט עורכי דין פליליים בתל אביב, אשר בטוחים שביכולתם להעניק ייעוץ וייצוג מקצועי מול המערכת הצבאית, אך בפועל לא מן הנמנע כי גם העורך הדין הנחשב ביותר בשוק לא יידע לייצג נאשמים כהלכה בתחום המשפט הצבאי.</p>
			<p>זאת, משום שהמערכת הצבאית והפרקליטות הצבאית שונות בתכלית ממקבילותיהן האזרחיות. בנוסף, דיני עבירות פליליות בצבא שונים לחלוטין מאלו אשר נידונים בבתי משפט "אזרחיים".</p>
			<p>עורך דין פלילי במרכז המתמחה בתחום הצבאי, וזהו תחום התמחות המרכזי עבורו, יידע לספק מעטפת של סיוע וטיפול מקצועי בערכאות הצבאיות בייצוג במגוון עבירות, החל משימוש בנשק באופן בלתי חוקי, עריקות, סחר באמל"ח, ועד לעבירות כמו עישון סמים, נפקדות ועוד.</p>
		</div>
	</div>
</template>

<style lang="scss">
@import '@/variables.scss';

#military-banner {
	width: 100%;
	height: 743px;
	background: url(../../../public/img/‏‏‏‏‏‏‏‏home/06/miitary-bg.jpg);
	background-size: contain;
	background-position: right;
	background-repeat: no-repeat;
	color: $main-color;
	margin-top: 50px;
	padding: 175px 14%;
	box-sizing: border-box;
	position: relative;

	#information-wrapper {
		width: 583px;
		height: 444px;
		overflow: auto;
		text-align: right;
		padding-right: 26px;
	

      &::-webkit-scrollbar {
        width: 1px;
      }
      &::-webkit-scrollbar-track-piece {
				background-color: #dfe0e0;
      }
      &::-webkit-scrollbar-thumb {
				background-color: #a8a8a8;
      }
	}

	.subtitle {
		font-family: $font-bold;
		font-size: 22px;
		line-height: 28px;
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

@media screen and (max-width: 500px) {
  #military-banner {
		height: 1120px;
		background-size: 715px auto;
		background-position: 70% bottom;
		background-repeat: no-repeat;
		margin: 0;
		padding: 160px 7%;

		#information-wrapper {
			width: 325px;
			height: 520px;
			padding-right: 15px;
		}

		.subtitle {
			font-family: $font-bold;
			font-size: 22px;
			line-height: 28px;
		}

		h2 {
			font-size: 36px;
			line-height: 36px;
		}
		
		p {
			font-size: 20px;
			line-height: 24px;
		}
	}
}
</style>