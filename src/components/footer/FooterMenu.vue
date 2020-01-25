<template>
	<div id="footer-menu" dir="rtl">
		<div class="footer-menu-list">
			<h4 class="list-title">עבירות פליליות</h4>
			<ul>
				<li><a href="#">עבירות שוד</a></li>
				<li><a href="#">עבירת הריגה</a></li>
				<li><a href="#">עבירות רכוש</a></li>
				<li><a href="#">עבירות מחשב</a></li>
				<li><a href="#">עבירות אלימות במשפחה</a></li>
				<li><a href="#">עבירות קניין רוחני</a></li>
				<li><a href="#">עבירות הימורים</a></li>
				<li><a href="#">עבירות זנות ותועבה</a></li>
			</ul>
		</div>
		<div class="footer-menu-list">
			<h4 class="list-title">משפט צבאי</h4>
			<ul>
				<li><a href="#">עבירות סמים בצבא</a></li>
				<li><a href="#">הטרדה מינית בצבא</a></li>
				<li><a href="#">פקודת הסמים המסוכנים</a></li>
				<li><a href="#">הסדרת מעמד נפקד, עריק ומשתמט</a></li>
				<li><a href="#">בדיקת סמים בצבא</a></li>
				<li><a href="#">שחרור מהצבא</a></li>
				<li><a href="#">מצ"ח</a></li>
				<li><a href="#">העדר הסכמה ומעשים מגונים</a></li>
			</ul>
		</div>
		<div class="footer-menu-list">
			<h4 class="list-title">משפט תעבורה</h4>
			<ul>
				<li><a href="#">נהיגה בשכרות</a></li>
				<li><a href="#">עבירת הפקרה</a></li>
				<li><a href="#">פסילה מנהלית</a></li>
				<li><a href="#">המרב"ד</a></li>
				<li><a href="#">נהיגה תחת השפעת סמים</a></li>
				<li><a href="#">נהיגה בקלות ראש</a></li>
				<li><a href="#">נהיגה במהירות מופרזת</a></li>
				<li><a href="#">שימוע בפני קצין משטרה</a></li>
			</ul>
		</div>
		<div class="footer-menu-list">
			<h4 class="list-title">חקירות ומעצרים</h4>
			<ul>
				<li><a href="#">חקירות במשטרה</a></li>
				<li><a href="#">מעצרים</a></li>
				<li><a href="#">שמירה על זכות השתיקה</a></li>
				<li><a href="#">ממעצר ימים ועד תום ההליכים</a></li>
				<li><a href="#">הדרך לביצוע מעצר</a></li>
				<li><a href="#">חיפוש לא חוקי</a></li>
				<li><a href="#">צו עיכוב יציאה מהארץ</a></li>
				<li><a href="#">מעצר בית</a></li>
			</ul>
		</div>
		<div class="footer-menu-list">
			<h4 class="list-title">תחומי עיסוק נוספים</h4>
			<ul>
				<li><a href="#">צו הרחקה, וצו למניעת הטרדה</a></li>
				<li><a href="#">טיעונים לעונש</a></li>
				<li><a href="#">ערעור פלילי</a></li>
				<li><a href="#">מחיקת רישום פלילי</a></li>
				<li><a href="#">רישום פלילי</a></li>
				<li><a href="#">כתב אישום פלילי</a></li>
				<li><a href="#">תעודת יושר</a></li>
				<li><a href="#">ועדת שחרורים</a></li>
			</ul>
		</div>
	</div>
</template>

<style lang="scss">
@import '@/variables.scss';

#footer-menu {
	width: 1364px;
	margin: 65px auto;
	@include flex;

	.footer-menu-list {
		width: 250px;
		height: 100%;
		@include flex(column, flex-start, flex-start);

		h4 {
			margin: 0;
			color: #1c1d21;
			font-family: $font-bold;
			font-size: 22px;
			font-weight: 400;
			position: relative;

			&::after {
				content: "";
				width: 200px;
				height: 0px;
				border-right: 50px solid #007eef;
				border-bottom: 1px solid rgba(185, 185, 185, 0.3);;
				position: absolute;
				right: 0;
				bottom: -30px;
			}
		}

		ul {
			margin-top: 50px;
			list-style-type: none;
			height: 296px;
			@include flex(column, flex-start, flex-start);
			
			a {
				color: #1c1d21;
				font-family: $font;
				font-size: 17px;
				font-weight: 400;
				line-height: 36px;
			}
		}
	}
}
@media screen and (max-width: 500px) {
  #footer-menu {
		display: none;
	} 
}
</style>