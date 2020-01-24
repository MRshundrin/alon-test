<template>
  <ul id="other-list">
		<li><a href="">צו הרחקה, וצו למניעת הטרדה</a></li>
		<li><a href="">טיעונים לעונש</a></li>
		<li><a href="">ערעור פלילי</a></li>
		<li><a href="">מחיקת רישום פלילי</a></li>
		<li><a href="">רישום פלילי</a></li>
		<li><a href="">כתב אישום פלילי</a></li>
		<li><a href="">תעודת יושר</a></li>
		<li><a href="">ועדת שחרורים</a></li>
		<li><a href="">חופשת אסירים</a></li>
		<li><a href="">עתירות אסירים</a></li>
		<li><a href="">הליכי שימוע</a></li>
		<li><a href="">הליכי הסגרה</a></li>
		<li><a href="">עבריינות נוער</a></li>
	</ul>
</template>


<style lang="scss">
@import '@/variables.scss';
#other-list {
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