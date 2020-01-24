<template>
  <div id="areas-section">
		<h2>תחומי עיסוקיו של עורך דין אלון ארז</h2>
		<div dir="rtl" id="areas-cards-wrapper">
			<div class="areas-card criminal-card" dir="rtl">
				<h3>הליך פלילי</h3>
				<p>משרד עורכי דין פליליים תל אביב אלון ארז מתמחה בייצוג חשודים ונאשמים בעבירות אלו במלוא המסירות.</p>
				<a href="">לפרטים <i class="fas fa-chevron-left"></i></a>
			</div>
			<div class="areas-card military-card" dir="rtl">
				<h3>הליך צבאי</h3>
				<p>עורך דין פלילי תל אביב אלון ארז יעניק לכל נאשם או לחשוד ליווי מקצועי מלא לאורך כל הדרך, משלב המעצר והייעוץ המשפטי הראשוני ועד להגשת ערעור בעת הצורך.</p>
				<a href="">לפרטים <i class="fas fa-chevron-left"></i></a>
			</div>
		</div>
	</div>
</template>


<style lang="scss">
@import '@/variables.scss';

#areas-section {
	padding: 140px 0 80px 0;
	@include flex(column);

	h2 {
		color: $main-color;
		font-family: $font-bold;
		font-size: 42px;
		line-height: 34px;
	}

	#areas-cards-wrapper {
		width: 1373px;
		margin-top: 50px;
		@include flex;
	}

	.areas-card {
		width: 672px;
		height: 386px;
		background: grey;
		padding: 20px 25px;
		box-sizing: border-box;
		position: relative;
		@include flex(column, flex-start, flex-start);

		h3 {
			color: $light-color;
			font-family: $font-bold;
			font-size: 48px;
			line-height: 34px;
			padding-bottom: 7px;
			border-bottom: 3px solid  #007eef;
			margin: 30px 0;
		}

		p {
			width: 350px;
			color: $light-color;
			font-size: 18px;
			line-height: 28px;
			letter-spacing: 0.2px;
		}

		a {
			width: 133px;
			height: 50px;
			background: rgba(255, 255, 255, 0.05);
			position: absolute;
			bottom: 30px;
			color: $light-color;
			font-family: $font-bold;
			font-size: 19px;
			text-align: center;
			box-sizing: border-box;
			padding: 13px 0;
			vertical-align: middle;	
			border: 1px solid #ffffff;
		}
	}

	.military-card {
		background: url(../../../public/img/‏‏‏‏‏‏‏‏home/02/army.png);
	}
	.criminal-card {
		background: url(../../../public/img/‏‏‏‏‏‏‏‏home/02/criminal.png);
	}

}

</style>