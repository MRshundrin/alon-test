<template>
  <ul id="traffic-list">
		<li><a href="">נהיגה בשכרות</a></li>
		<li><a href="">עבירת הפקרה</a></li>
		<li><a href="">פסילה מנהלית</a></li>
		<li><a href="">המרב"ד</a></li>
		<li><a href="">נהיגה תחת השפעת סמים</a></li>
		<li><a href="">נהיגה בקלות ראש</a></li>
		<li><a href="">נהיגה במהירות מופרזת</a></li>
		<li><a href="">אי ציות לרמזור אדום</a></li>
		<li><a href="">נהיגה ללא רישיון</a></li>
		<li><a href="">שימוע בפני קצין משטרה</a></li>
		<li><a href="">נהיגה בזמן פסילה</a></li>
	</ul>
</template>


<style lang="scss">
@import '@/variables.scss';
#traffic-list {
	list-style-type: none;
	padding: 25px 25px 0 25px;
	

	li :before {
		content:">";
		margin-left: 20px;
	}
	
	li :hover::before {
		color: #007eef;
	}
}
</style>