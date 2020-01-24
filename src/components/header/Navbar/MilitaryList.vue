<template>
  <ul id="military-list">
		<li><a href="">עבירות סמים בצבא</a></li>
		<li><a href="">הטרדה מינית בצבא</a></li>
		<li><a href="">פקודת הסמים המסוכנים</a></li>
		<li><a href="">הסדרת מעמד נפקד, עריק ומשתמט</a></li>
		<li><a href="">בדיקת סמים בצבא</a></li>
		<li><a href="">שחרור מהצבא</a></li>
		<li><a href="">מצ"ח</a></li>
		<li><a href="">העדר הסכמה ומעשים מגונים</a></li>
		<li><a href="">עריקות</a></li>
		<li><a href="">פטור משירות מילואים</a></li>
		<li><a href="">מחיקת רישום מלפני הגיוס</a></li>
		<li><a href="">עבירות אלימות בצבא</a></li>
	</ul>
</template>


<style lang="scss">
@import '@/variables.scss';
#military-list {
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