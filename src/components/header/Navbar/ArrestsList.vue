<template>
  <ul id="arrests-list">
		<li><a href="">חקירות במשטרה</a></li>
		<li><a href="">מעצרים</a></li>
		<li><a href="">שמירה על זכות השתיקה</a></li>
		<li><a href="">ממעצר ימים ועד תום ההליכים</a></li>
		<li><a href="">הדרך לביצוע מעצר</a></li>
		<li><a href="">חיפוש לא חוקי</a></li>
		<li><a href="">צו עיכוב יציאה מהארץ</a></li>
		<li><a href="">מעצר בית</a></li>
	</ul>
</template>

<style lang="scss">
@import '@/variables.scss';

#arrests-list {
	list-style-type: none;

	li :before {
		content:">";
		margin-left: 20px;
	}

	li :hover::before {
		color: #007eef;
	}
}

</style>