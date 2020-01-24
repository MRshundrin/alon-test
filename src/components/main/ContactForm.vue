<template>
	<div id="form-section">
		<div id="form-info">
			<div id="left-part">
				<p id="form-title">או השאירו פרטים לקבלת שיחה חוזרת</p>
				<form action="submit" dir="rtl" id="form">
					<input type="text" placeholder="שם מלא *">
					<input type="text" placeholder="נייד *">
					<select name="time select">
						<option value="placeholder" selected>בחר שעה לחזרה</option> 
						<option value="morning">Morning</option>
						<option value="day">Day</option>
						<option value="evening">Evening</option>
					</select>
					<button>תחזרו אליי <i class="fas fa-chevron-left"></i></button>
				</form>
			</div>
			<div id="contact-information">
				<span id="phone-number">050-7368203</span>
				<img src="img/‏‏‏‏‏‏‏‏home/01/3layers.png" alt="phone">
				<div>
					<p>זמין <span>24 שעות</span> ביממה</p>
					<p>לייעוץ ראשוני חייגו</p>
				</div>
			</div>
		</div>
	</div>
</template>

<style lang="scss">
@import '@/variables.scss';

#form-section {
	width: 1371px;
	margin: 0 auto;
	background: $light-color;
	padding: 30px 0;
	@include flex(column);
	position: absolute;
	top: 613px;
	left: 0;
	right: 0;
	margin: auto;
	box-shadow: 0 8px 84px rgba(83, 103, 118, 0.13);

	#form-title {
		color: $text-color;
		font-size: 22px;
	}

	#form-info {
		@include flex;

		#left-part {
			@include flex(column, space-between, flex-end);
			margin-right: 30px;
		}
	}

	#contact-information {
		@include flex;

		div {
			@include flex(column);

			p:first-child {
				color: #007eef;
				font-family: $font-bold;
				font-size: 30px;
				
				span {
					color: $main-color;
				}
			}

			p:last-child {
				color: $main-color;
				font-size: 30px;
			}
		}

		#phone-number {
			color: $main-color;
			font-family: $font-bold;
			font-size: 40px;
		}
	}

	#form {
		width: 720px;
		@include flex;

		input {
			width: 177px;
			height: 44px;
			background-color: #f3f6f8;
			color: #454545;
			font-family: $font;
			font-size: 17px;
			border: none;
			padding-right: 15px;

			&::placeholder {
				color: #454545
			}
		}

		select {
			width: 177px;
			height: 44px;
			background-color: #f3f6f8;
			border: none;
			color: #454545;
			font-size: 17px;
		}

		button {
			width: 147px;
			height: 44px;
			background-color: #007eef;
			border: none;
			padding: 0;
			color: #ffffff;
			font-family: $font-bold;
			font-size: 19px;

			i {
				font-size: 9px;
			}
		}
	}
}
</style>