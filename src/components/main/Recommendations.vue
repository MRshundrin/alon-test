<template>
  <div id="recommendations-wrapper">
    <h2>המלצות</h2>
    <div id="recommendations-content" dir="rtl">
      <button @click="refresh"><i class="fas fa-chevron-right"></i></button>
        <div class="recommendations">
          <div class="recommendation-card" v-if="counter == 1">
            <div class="recommendation-card-feedback">
              <div class="recommendation-card-feedback-header">
                <img src="img/‏‏‏‏‏‏‏‏home/03/google-logo.png" alt="google-logo">
                <img src="img/‏‏‏‏‏‏‏‏home/03/quote.png" alt="quote">
              </div>
              <span><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i></span>
              <div class="paragraph-wrapper">
                <p>
                  חיפשנו עורך דין הוגן. מצאנו. אישתי פרסמה בקבוצה בפייסבוק. עורך דין אלון ארז השיב במהרה. תוך שעתיים הגענו אליו.עורך דין פלילי אדיב, נעים, מקשיב, מפגין ידע רב ומקצועי.מרגיע והכי חשוב הוגן. בהחלט מהטובים והמומלצים ביותרחיפשנו עורך דין הוגן. מצאנו. אישתי פרסמה בקבוצה בפייסבוק. עורך דין אלון ארז השיב במהרה. תו
                </p>
              </div>
            </div>
            <div class="recommendation-card-footer">
              <img src="img/‏‏‏‏‏‏‏‏home/03/avatar4.png" alt="avatar">
              <div>
                <p class="name">Amit Green Photographer</p>
                <p class="date">לפני שבועיים</p>
              </div>
            </div>
          </div>

          <div class="recommendation-card" v-if="counter == 1">
            <div class="recommendation-card-feedback">
              <div class="recommendation-card-feedback-header">
                <img src="img/‏‏‏‏‏‏‏‏home/03/google-logo.png" alt="google-logo">
                <img src="img/‏‏‏‏‏‏‏‏home/03/quote.png" alt="quote">
              </div>
              <span><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i></span>
              <div class="paragraph-wrapper">
                <p>עוד מקצועי ,אלוף, יודע להקשיב,לתמוך , לתת כתף ,להפנות לאן שצריך ונותן מענה לא רק לעניין הספציפי שהוא מתמחה בו . ממליץ בחום.</p>
              </div>
            </div>
            <div class="recommendation-card-footer">
              <img src="img/‏‏‏‏‏‏‏‏home/03/avatar3.png" alt="avatar">
              <div>
                <p class="name">שלומית מזרחי</p>
                <p class="date">לפני שבועיים</p>
              </div>
            </div>
          </div>

          <div class="recommendation-card" v-if="counter == 1">
            <div class="recommendation-card-feedback">
              <div class="recommendation-card-feedback-header">
                <img src="img/‏‏‏‏‏‏‏‏home/03/google-logo.png" alt="google-logo">
                <img src="img/‏‏‏‏‏‏‏‏home/03/quote.png" alt="quote">
              </div>
              <span><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i></span>
              <div class="paragraph-wrapper">
                <p>עורך דין ובן אדם מדהים. לא האמנתי שיצליח לזכות את הבן שלי, אחרי שהסניגור הציבורי המליץ לנו לההודות. פשוט מדהים!!!</p>
              </div>
            </div>
            <div class="recommendation-card-footer">
              <img src="img/‏‏‏‏‏‏‏‏home/03/avatar2.png" alt="avatar">
              <div>
                <p class="name">סבטלנה</p>
                <p class="date">לפני שבועיים</p>
              </div>
            </div>
          </div>

          <div class="recommendation-card" v-if="counter == 1">
            <div class="recommendation-card-feedback">
              <div class="recommendation-card-feedback-header">
                <img src="img/‏‏‏‏‏‏‏‏home/03/google-logo.png" alt="google-logo">
                <img src="img/‏‏‏‏‏‏‏‏home/03/quote.png" alt="quote">
              </div>
              <span><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i></span>
              <div class="paragraph-wrapper">
                <p>Alon helped me settle my military status from overseas after I had a couple failed attempts trying to deal with the embassy by myself. Good email communication. Quick and easy</p>
              </div>
            </div>
            <div class="recommendation-card-footer">
              <img src="img/‏‏‏‏‏‏‏‏home/03/avatar1.png" alt="avatar">
              <div>
                <p class="name">Matan Hershberg</p>
                <p class="date">לפני שבועיים</p>
              </div>
            </div>
          </div>

          <div class="recommendation-card" v-if="counter == 2">
            <div class="recommendation-card-feedback">
              <div class="recommendation-card-feedback-header">
                <img src="img/‏‏‏‏‏‏‏‏home/03/google-logo.png" alt="google-logo">
                <img src="img/‏‏‏‏‏‏‏‏home/03/quote.png" alt="quote">
              </div>
              <span><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i></span>
              <div class="paragraph-wrapper">
                <p>
                  חיפשנו עורך דין הוגן. מצאנו. אישתי פרסמה בקבוצה בפייסבוק. עורך דין אלון ארז השיב במהרה. תוך שעתיים הגענו אליו.עורך דין פלילי אדיב, נעים, מקשיב, מפגין ידע רב ומקצועי.מרגיע והכי חשוב הוגן. בהחלט מהטובים והמומלצים ביותרחיפשנו עורך דין הוגן. מצאנו. אישתי פרסמה בקבוצה בפייסבוק. עורך דין אלון ארז השיב במהרה. תו
                </p>
              </div>
            </div>
            <div class="recommendation-card-footer">
              <img src="img/‏‏‏‏‏‏‏‏home/03/avatar1.png" alt="avatar">
              <div>
                <p class="name">Amit Green Photographer</p>
                <p class="date">לפני שבועיים</p>
              </div>
            </div>
          </div>

          <div class="recommendation-card" v-if="counter == 2">
            <div class="recommendation-card-feedback">
              <div class="recommendation-card-feedback-header">
                <img src="img/‏‏‏‏‏‏‏‏home/03/google-logo.png" alt="google-logo">
                <img src="img/‏‏‏‏‏‏‏‏home/03/quote.png" alt="quote">
              </div>
              <span><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i></span>
              <div class="paragraph-wrapper">
                <p>
                  חיפשנו עורך דין הוגן. מצאנו. אישתי פרסמה בקבוצה בפייסבוק. עורך דין אלון ארז השיב במהרה. תוך שעתיים הגענו אליו.עורך דין פלילי אדיב, נעים, מקשיב, מפגין ידע רב ומקצועי.מרגיע והכי חשוב הוגן. בהחלט מהטובים והמומלצים ביותרחיפשנו עורך דין הוגן. מצאנו. אישתי פרסמה בקבוצה בפייסבוק. עורך דין אלון ארז השיב במהרה. תו
                </p>
              </div>
            </div>
            <div class="recommendation-card-footer">
              <img src="img/‏‏‏‏‏‏‏‏home/03/avatar4.png" alt="avatar">
              <div>
                <p class="name">שלומית מזרחי</p>
                <p class="date">לפני שבועיים</p>
              </div>
            </div>
          </div>

          <div class="recommendation-card" v-if="counter == 2">
            <div class="recommendation-card-feedback">
              <div class="recommendation-card-feedback-header">
                <img src="img/‏‏‏‏‏‏‏‏home/03/google-logo.png" alt="google-logo">
                <img src="img/‏‏‏‏‏‏‏‏home/03/quote.png" alt="quote">
              </div>
              <span><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i></span>
              <div class="paragraph-wrapper">
                <p>
                  חיפשנו עורך דין הוגן. מצאנו. אישתי פרסמה בקבוצה בפייסבוק. עורך דין אלון ארז השיב במהרה. תוך שעתיים הגענו אליו.עורך דין פלילי אדיב, נעים, מקשיב, מפגין ידע רב ומקצועי.מרגיע והכי חשוב הוגן. בהחלט מהטובים והמומלצים ביותרחיפשנו עורך דין הוגן. מצאנו. אישתי פרסמה בקבוצה בפייסבוק. עורך דין אלון ארז השיב במהרה. תו
                </p>
              </div>
            </div>
            <div class="recommendation-card-footer">
              <img src="img/‏‏‏‏‏‏‏‏home/03/avatar2.png" alt="avatar">
              <div>
                <p class="name">Amit Green Photographer</p>
                <p class="date">לפני שבועיים</p>
              </div>
            </div>
          </div>

          <div class="recommendation-card" v-if="counter == 2">
            <div class="recommendation-card-feedback">
              <div class="recommendation-card-feedback-header">
                <img src="img/‏‏‏‏‏‏‏‏home/03/google-logo.png" alt="google-logo">
                <img src="img/‏‏‏‏‏‏‏‏home/03/quote.png" alt="quote">
              </div>
              <span><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i></span>
              <div class="paragraph-wrapper">
                <p>
                  חיפשנו עורך דין הוגן. מצאנו. אישתי פרסמה בקבוצה בפייסבוק. עורך דין אלון ארז השיב במהרה. תוך שעתיים הגענו אליו.עורך דין פלילי אדיב, נעים, מקשיב, מפגין ידע רב ומקצועי.מרגיע והכי חשוב הוגן. בהחלט מהטובים והמומלצים ביותרחיפשנו עורך דין הוגן. מצאנו. אישתי פרסמה בקבוצה בפייסבוק. עורך דין אלון ארז השיב במהרה. תו
                </p>
              </div>
            </div>
            <div class="recommendation-card-footer">
              <img src="img/‏‏‏‏‏‏‏‏home/03/avatar3.png" alt="avatar">
              <div>
                <p class="name">Matan Hershberg</p>
                <p class="date">לפני שבועיים</p>
              </div>
            </div>
          </div>
        </div>
        <div class="recomendations-mobile">
          <div class="recommendation-card" v-if="counter == 1">
            <div class="recommendation-card-feedback">
              <div class="recommendation-card-feedback-header">
                <img src="img/‏‏‏‏‏‏‏‏home/03/google-logo.png" alt="google-logo">
                <img src="img/‏‏‏‏‏‏‏‏home/03/quote.png" alt="quote">
              </div>
              <span><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i></span>
              <div class="paragraph-wrapper">
                <p>
                  חיפשנו עורך דין הוגן. מצאנו. אישתי פרסמה בקבוצה בפייסבוק. עורך דין אלון ארז השיב במהרה. תוך שעתיים הגענו אליו.עורך דין פלילי אדיב, נעים, מקשיב, מפגין ידע רב ומקצועי.מרגיע והכי חשוב הוגן. בהחלט מהטובים והמומלצים ביותרחיפשנו עורך דין הוגן. מצאנו. אישתי פרסמה בקבוצה בפייסבוק. עורך דין אלון ארז השיב במהרה. תו
                </p>
              </div>
            </div>
            <div class="recommendation-card-footer">
              <img src="img/‏‏‏‏‏‏‏‏home/03/avatar4.png" alt="avatar">
              <div>
                <p class="name">Amit Green Photographer</p>
                <p class="date">לפני שבועיים</p>
              </div>
            </div>
          </div>

          <div class="recommendation-card" v-if="counter == 2">
            <div class="recommendation-card-feedback">
              <div class="recommendation-card-feedback-header">
                <img src="img/‏‏‏‏‏‏‏‏home/03/google-logo.png" alt="google-logo">
                <img src="img/‏‏‏‏‏‏‏‏home/03/quote.png" alt="quote">
              </div>
              <span><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i></span>
              <div class="paragraph-wrapper">
                <p>עוד מקצועי ,אלוף, יודע להקשיב,לתמוך , לתת כתף ,להפנות לאן שצריך ונותן מענה לא רק לעניין הספציפי שהוא מתמחה בו . ממליץ בחום.</p>
              </div>
            </div>
            <div class="recommendation-card-footer">
              <img src="img/‏‏‏‏‏‏‏‏home/03/avatar3.png" alt="avatar">
              <div>
                <p class="name">שלומית מזרחי</p>
                <p class="date">לפני שבועיים</p>
              </div>
            </div>
          </div>
        </div>
      <button @click="refresh"><i class="fas fa-chevron-left"></i></button>
    </div>
    <div class="dot-section">
      <div class="dot" :class="{ active: counter == 1 }"></div>
      <div class="dot" :class="{ active: counter == 2 }"></div>
    </div>
  </div>
</template>

<script>

  export default {
    name: 'recomendation',
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

#recommendations-wrapper {
  height: 585px;
  background-image: linear-gradient(to top, #ffffff 0%, #eaeff3 100%);
  
  @include flex(column, space-around, center);

  h2 {
    color: $main-color;
    font-family: $font-bold;
    font-size: 42px;
    font-weight: 400;
  }
}

#recommendations-content {
  width: 1500px;
  @include flex;

  button {
    border: none;
    width: 46px;
    height: 46px;
    background-color: #dee7ed;
    color: #007eef;
    font-weight: 100;
    font-size: 20px;
  }
}

.recommendations {
  @include flex;
  width: 1371px;
}

.recomendations-mobile {
  display: none;
}

.recommendation-card {
  width: 320px;
  @include flex (column, space-between, flex-start);
  box-sizing: border-box;

  &-feedback {
    width: 320px;
    height: 303px;
    @include flex(column, flex-start, flex-start);
    background: $light-color;
    padding: 30px;
    margin-bottom: 40px;
    box-sizing: border-box;
    position: relative;

    &-header {
      width: 100%;
      @include flex;
      margin-bottom: 10px;
    }

    i {
      font-size: 16px;
      color: #007eef;
      letter-spacing: 5px;
    }

    .paragraph-wrapper {
      height: 151px;
      overflow: auto;

      &::-webkit-scrollbar {
        width: 2px;
      }
      &::-webkit-scrollbar-track-piece {
        background-color: #c1cad3;
      }
      &::-webkit-scrollbar-thumb {
        background-color: #00274e;
      }  
    }

    p {
      margin-top: 25px;
      width: 261px;
      color: $second-color;
      font-family: $font;
      font-size: 17px;
    }

    &::after {
      content: ''; 
      position: absolute; 
      left: 258px; bottom: -30px; 
      border: 15px solid transparent;
      border-top: 15px solid white;
    }
  }

  &-footer {
    @include flex(row, flex-start, center);

    .name {
      color: $main-color;
      font-family: $font-bold;
      font-size: 20px;
      line-height: 33.11px;
    }
    .date {
      color: $second-color;
      font-family: $font;
      font-size: 16px;
      font-weight: 300;
      line-height: 17.53px;
    }

    img {
      margin-left: 5px;
    }
  }
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

@media screen and (max-width: 500px) {
  #recommendations-wrapper {
    height: 520px;
    background-image: linear-gradient(to top, #ffffff 0%, #eaeff3 100%);
    
    @include flex(column, space-around, center);

    h2 {
      font-size:  36px; 
    }
  }

  #recommendations-content {
    width: 100%;
    @include flex;

    button {
			width: 36px;
		}
  }

  .recommendations {
    display: none;
  }

  .recomendations-mobile {
    @include flex;
    width: 287px;

    .recommendation-card {
      width: 100%;
      

      &-feedback {
        width: 100%;
        height: 287px;
        padding: 25px;
        margin-bottom: 28px;

        p {
          margin-top: 20px;
          width: 230px;
          font-size: 16px;
        }

        &::after {
          left: 230px; bottom: -30px; 
        }
      }

      &-footer {
        @include flex(row, flex-start, center);

        .name {
          font-size: 17px;
          line-height: 33.11px;
        }
        .date {
          font-size: 15px;
        }
      }
    }
  }
}

</style>

