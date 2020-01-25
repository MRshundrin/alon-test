<template>
	<div id="videos-wrapper" dir="rtl">
		<h2>פרסומים וראיונות בטלוויזיה</h2>
		<div id="videos-slider-wrapper">
			<div id="videos-slider-content">
				<button @click="refresh"><i class="fas fa-chevron-right"></i></button>
				<div class="videos-slider">
					<div class="videos-slider-card" v-if="counter == 1">
						<div class="video-screenshot first-video">
							<button><i class="fas fa-play"></i></button>
						</div>
						<p class="video-views">כאן 11</p>
						<p class="video-name">עבירות אלימות במשפחה - מגיעים מוכנים לחקירה - עורך דין פלילי אלון ארז</p>
					</div>

					<div class="videos-slider-card" v-if="counter == 1">
						<div class="video-screenshot second-video">
							<button><i class="fas fa-play"></i></button>
						</div>
						<p class="video-views">חדשות 10</p>
						<p class="video-name">קנסות לצרכי זנות - עו"ד אלון ארז</p>
					</div>

					<div class="videos-slider-card" v-if="counter == 1">
						<div class="video-screenshot third-video">
							<button><i class="fas fa-play"></i></button>
						</div>
						<p class="video-views">ערוץ 2</p>
						<p class="video-name">חייל בצה"ל - חוקרי מצ"ח מזמנים אותך לחקירה בחשד לעבירות סמים, מה תעשה?</p>
					</div>

					<div class="videos-slider-card" v-if="counter == 2">
						<div class="video-screenshot third-video">
							<button><i class="fas fa-play"></i></button>
						</div>
						<p class="video-views">ערוץ 2</p>
						<p class="video-name">חייל בצה"ל - חוקרי מצ"ח מזמנים אותך לחקירה בחשד לעבירות סמים, מה תעשה?</p>
					</div>

					<div class="videos-slider-card" v-if="counter == 2">
						<div class="video-screenshot first-video">
							<button><i class="fas fa-play"></i></button>
						</div>
						<p class="video-views">כאן 11</p>
						<p class="video-name">עבירות אלימות במשפחה - מגיעים מוכנים לחקירה - עורך דין פלילי אלון ארז</p>
					</div>

					<div class="videos-slider-card" v-if="counter == 2">
						<div class="video-screenshot second-video">
							<button><i class="fas fa-play"></i></button>
						</div>
						<p class="video-views">חדשות 10</p>
						<p class="video-name">קנסות לצרכי זנות - עו"ד אלון ארז</p>
					</div>
				</div>
				<div class="videos-slider-mobile">
					<div class="videos-slider-card" v-if="counter == 1">
						<div class="video-screenshot first-video">
							<button><i class="fas fa-play"></i></button>
						</div>
						<p class="video-views">כאן 11</p>
						<p class="video-name">עבירות אלימות במשפחה - מגיעים מוכנים לחקירה - עורך דין פלילי אלון ארז</p>
					</div>

					<div class="videos-slider-card" v-if="counter == 2">
						<div class="video-screenshot second-video">
							<button><i class="fas fa-play"></i></button>
						</div>
						<p class="video-views">חדשות 10</p>
						<p class="video-name">קנסות לצרכי זנות - עו"ד אלון ארז</p>
					</div>
				</div>
				<button @click="refresh"><i class="fas fa-chevron-left"></i></button>
			</div>
			<div class="dot-section">
				<div class="dot" :class="{ active: counter == 1 }"></div>
				<div class="dot" :class="{ active: counter == 2 }"></div>
			</div>
		</div>
	</div>
</template>

<script>

	export default {
		name: 'VideoSection',
		data: () => ({
      counter: 1
    }),
    methods: {
      refresh () {
        if (this.counter == 1) {
          this.counter = 2
        } else {
          this.counter = 1
        }
      }
    }
	}
</script>

<style lang="scss">
@import '@/variables.scss';

#videos-wrapper {
	@include flex(column, flex-start);
	background-color: #20222c;
	width: 100%;
	height: 621px;

	h2 {
		color: $light-color;
		font-family: $font-bold;
		font-size: 48px;
		margin: 70px auto 40px auto;
	}
}

#videos-slider-wrapper {
	height: 390px;
	@include flex(column);


	#videos-slider-content {
		width: 1500px;
		@include flex(row, space-between, baseline);
	}

	.videos-slider-mobile {
		display: none;
	}

	.videos-slider {
		width: 1371px;
		@include flex;

		&-card {
			width: 422px;
			height: 351px;
			@include flex(column, flex-start, flex-start);

			.video-views {
				opacity: 0.25;
				color: $light-color;
				font-size: 18px;
				font-weight: 700;
				padding: 24px 0 15px 0;
				align-self: stretch;
				border-bottom: 1px solid #5a5959;
			}

			.video-name {
				@include flex;
				color: $light-color;
				font-size: 24px;
				font-weight: 300;
				line-height: 28px;
				height: 50px;
				margin-top: 15px;
			}

			.video-screenshot {
				width: 421px;
				height: 236px;
				background-size: cover;
				background-repeat: no-repeat;
				@include flex(row, center, center);

				button {
					width: 62px;
					height: 62px;
					border: 1px solid rgba(255, 255, 255, 0.6);;
					background-color: rgba(0, 0, 0, 0.2);
					text-shadow: white 1px 0 0, white -1px 0 0, white -1px 0 0, white 1px 0 0;
					font-size: 20px;
					color: #007eef;
					padding: 20px;
					box-sizing: border-box;
				}
			}

			.first-video {
				background: url(../../../public/img/‏‏‏‏‏‏‏‏home/06/first_video.png);
			}

			.second-video {
				background: url(../../../public/img/‏‏‏‏‏‏‏‏home/06/second_video.png);
			}

			.third-video {
				background: url(../../../public/img/‏‏‏‏‏‏‏‏home/06/third_video.png);
			}
		}	
	}
	
	button {
    border: none;
    width: 46px;
    height: 46px;
    background-color: #3a3d4b;
    color: $light-color;
    font-weight: 100;
    font-size: 20px;
	}
	.dot-section {
		@include flex;
		width: 41px;

		.dot {
			width: 9px;
			height: 9px;
			background-color: #dee7ed;
		}
		
		.active {
			background-color: #007eef;
		}
	}
}

@media screen and (max-width: 500px) {
  #videos-wrapper {
		width: 100%;
		height: 475px;

		h2 {
			font-size: 36px;
			line-height: 30px;
			margin: 56px auto 35px auto;
			text-align: center;
		}
	}

	#videos-slider-wrapper {
		width: 100%;
		height: 275px;

		#videos-slider-content {
			width: 100%;
			height: 100%;
		}

		.videos-slider-mobile {
			display: block;
			.videos-slider-card {
				width: 286px;
				height: 260px;

				.video-views {
					font-size: 16px;
					padding: 10px 0;
				}

				.video-name {
					font-size: 20px;
					margin: 0;
					line-height: 15px;
				}

				.video-screenshot {
					width: 286px;
					height: 161px;
					background-size: cover;

					button {
						width: 50px;
						height: 52px;
						padding: 14px;
					}
				}
			}	
		}

		.videos-slider {
			display: none;
		}
		
		button {
			width: 36px;
		}
	}
}
</style>