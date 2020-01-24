<template>
  <ul id="criminal-list">
		<li><a href="">עבירות שוד</a></li>
		<li><a href="">עבירת הריגה</a></li>
		<li><a href="">עבירות רכוש</a></li>
		<li><a href="">עבירות מחשב</a></li>
		<li><a href="">עבירות אלימות במשפחה</a></li>
		<li><a href="">עבירות קניין רוחני</a></li>
		<li><a href="">עבירות הימורים</a></li>
		<li><a href="">עבירות זנות ותועבה</a></li>
		<li><a href="">העלבת עובד ציבור</a></li>
		<li><a href="">עבירות הונאה</a></li>
		<li><a href="">עבירות מין</a></li>
		<li><a href="">עבירות סמים</a></li>
		<li><a href="">הגנת פרטיות</a></li>
		<li><a href="">קבלת דבר במרמה</a></li>
		<li><a href="">האזנת סתר</a></li>
		<li><a href="">החזקת סכין</a></li>
		<li><a href="">הטרדה מינית</a></li>
		<li><a href="">התחזות</a></li>
		<li><a href="">עבירות נשק</a></li>
		<li><a href="">עבירת רצח</a></li>
		<li><a href="">עבירות אלימות ואיומים</a></li>
		<li><a href="">לשון הרע</a></li>
		<li><a href="">הטרדה מינית בעבודה</a></li>
		<li><a href="">צווארון לבן</a></li>
		<li><a href="">הימורים באינטרנט</a></li>
		<li><a href="">עבירות מין באינטרנט</a></li>
		<li><a href="">סחר בבני אדם</a></li>
		<li><a href="">הברחת סמים מחו"ל</a></li>
	</ul>
</template>

<style lang="scss">
@import '@/variables.scss';

#criminal-list {
	height: 361px;
	width: 100%;
	padding: 0;
	list-style-type: none;
	column-count: 2;

	li :before {
		content:">";
		margin-left: 20px;
	}

	li :hover::before {
		color: #007eef;
	}	
}

</style>