<template>
	<div id="banner" dir="rtl">
		<h1 id="banner-title">עורך דין פלילי אלון ארז</h1>
		<h2 id="description">ייעוץ וייצוג נאשמים וחשודים במשפט הפלילי</h2>
		<ul id="description-list">
			<li><span>ייעוץ אישי</span></li>
			<li><span>מאוד לקוחות מרוצים</span></li>
			<li><span>הצלחות והישגים חסרי תקדים</span></li>
		</ul>
		<button id="call-button"><img src="img/‏‏‏‏‏‏‏‏home/01/4layers.png" alt=""></button>
	</div>
</template>

<style lang="scss">
@import '@/variables.scss';

#call-button {
	background: transparent;
	border: none;
	outline: none;
	position: absolute;
	right: 0px;
	bottom: -50px;
}

#banner {
	height: 680px;
	background: url(../../../public/img/‏‏‏‏‏‏‏‏home/01/banner_main.jpg);
	background-size: cover;
	background-repeat: no-repeat;
	background-color: black;
	color: $light-color;
	padding: 170px 14%;
	box-sizing: border-box;
	position: relative;

	#banner-title {
		font-family: $font-bold;
		font-size: 62px;
	}
	#description {
		font-size: 34px;
			font-weight: 300;
	}
	#description-list {
		font-size: 28px;
		font-weight: 300;
		line-height: 40px;
		list-style-type: square;
		color: #007eef;

		span {
			color: $light-color;
		}
	}
}

@media screen and (max-width: 500px) {
  #call-button {
		display: none;
	}

	#banner {
		height: 580px;
		background-size: cover;
		background-position: 34% 30%;
		background: url(../../../public/img/‏‏‏‏‏‏‏‏home/01/banner-mobile.png);
		background-repeat: no-repeat;
		background-size: cover;
		padding: 323px 15px 54px 15px;


		#banner-title {
			font-size: 38px;
			line-height: 38px;
		}
		#description {
			font-size: 28px;
			font-weight: 300;
		}
		#description-list {
			font-size: 20px;
			font-weight: 300;
			line-height: 32px;
			margin-right: 15px;
		}
	}
}
</style>