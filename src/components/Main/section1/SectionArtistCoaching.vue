<template>
  <!-- ac = ArtistCoaching  per identificare la sezione -->
  <div>

    <div class="container-section-ac">

      <div class="info-hero">
        <span>
          Artist coaching
        </span> 
        <span>
          I understand what it takes to create. I can help you with
        </span>
      </div> 
      
      <div class="ac-card">
        <div v-for="(skils, index) in skilsList" :key="index">
          <img :src='"../../../images/artist-box-image-" + skils.img + ".png"' alt="">
          <span>{{skils.title}}</span>
          <p>{{skils.description}}</p>
        </div> 
      </div>
  
      <div class="ac-info">
        <div class="info-sx">
          <img src="@/images/artist-quote-icon.png" alt="">
          <p>I coach and mentor visual artist, like you, to Create Like You Mean It</p>
          <span>Martin Garrix</span>
        </div>
  
        <div class="info-dx">
          <p>As a coach and mentor, my ultimate goal is to motivate visual artist toward inspired action, I help you get you back on track to being the productive, creative, meaningful and authentic artist you truly want to be. I support artist in crafting and living a creative life as well as feeling good about themselves and thei art.</p>
          <p>As an artist and an educator for nearly 30 years, i understand what it takess to create.</p>
          <button>Get started today</button>
        </div>
  
      </div>

    </div>

    <div class="ac-img">
      <img src="@/images/artist-video-poster.jpg" alt="">
      <a href="" class="ac-play">
        <img src="@/images/icon-youtube-play.png" alt="">
      </a>
    </div>

    <div class="title-testimonial">
      <span>
        Testimonial
      </span> 
      <span>
        Why do people love me?
      </span>
    </div>

    <div class="card-testimonial">
      <div v-for="(testimonial, index) in cardTestimonialList" :key="index" class="testimonial">
        <span>{{testimonial.title}}</span>
        <p>{{testimonial.description}}</p>
        <div>
          <img :src='"@/images/artist-testimonial-avatar-" + testimonial.img + ".jpg"' alt="">
          <span>{{testimonial.name}}</span>
          <span>{{testimonial.profession}}</span>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
export default {
  name:  'SectionArtistCoaching',

  data(){
    return{
      skilsList:[
        {
          img:'01',
          title: 'Online Coures',
          description: 'Online art coaching now offers you a very powerful way to redesing your artist mind.'
        },
        {
          img:'02',
          title: 'One to One',
          description: 'Getting the necessary clarity about the current state to help you improve your ability.'
        },
        {
          img:'03',
          title: 'Anywhere',
          description: 'Access to valuable and portable program which allow you to step and live anywhere you want.'
        },
        {
          img:'04',
          title: 'On Time',
          description: 'Punctualy i our priority beacause it`s an essential to assess a program quality.'
        }
      ],
      cardTestimonialList:[
        {
          img:'01',
          title: 'High level of efficiency and scientific teaching methods',
          description: 'i am ffree to learn at my own pace, follow my own sschedule and choose the subject i want to learn from the syllabuss. Great study portal for people like me.',
          name: 'Mina Hollace',
          profession: '/Freelancer'
        },
        {
          img:'02',
          title: 'High level of efficiency and scientific teaching methods',
          description: 'i am ffree to learn at my own pace, follow my own sschedule and choose the subject i want to learn from the syllabuss. Great study portal for people like me.',
          name: 'Mina Hollace',
          profession: '/Freelancer'
        },
        {
          img:'03',
          title: 'High level of efficiency and scientific teaching methods',
          description: 'i am ffree to learn at my own pace, follow my own sschedule and choose the subject i want to learn from the syllabuss. Great study portal for people like me.',
          name: 'Mina Hollace',
          profession: '/Freelancer'
        },
        {
          img:'04',
          title: 'High level of efficiency and scientific teaching methods',
          description: 'i am ffree to learn at my own pace, follow my own sschedule and choose the subject i want to learn from the syllabuss. Great study portal for people like me.',
          name: 'Mina Hollace',
          profession: '/Freelancer'
        },
      ]
    }
  }
}
</script>

<style  lang="scss">
.container-section-ac{
  width: 1070px;
  margin: 0 auto;

  .info-hero{
      display: flex;
      flex-direction: column;
      align-items: center;
      margin: 100px 0;
    }
  .ac-card{
    display: flex;
    justify-content: center;
    margin: 100px 0;

      div{

        width: calc(100%/4);
        display: flex;
        flex-direction: column;

        img{
          width: 100px;
        }
      }
  } 
  .ac-info{
    display: flex;
    justify-content: space-between;
      .info-sx{
        display: flex;
        flex-direction: column;
        align-items: center;
        text-align: center;
          img{
            width: 30px;
          }
      }
      .info-dx{
        width: 500px;
          p{
            padding: 10px 0;
          }
      }
  }
}
.ac-img{
  display: flex;
  justify-content: center;
  margin-top: 110px;
  position: relative;

   .ac-play{
      position: absolute;
      top: 50%;
   }
}

.title-testimonial{
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  margin: 110px 0;
}
.card-testimonial{

  display: flex;
  justify-content: space-around;

  .testimonial{
    width: 500px;
    padding: 25px;
    background-color: aquamarine;
  }

    img{
      height: 70px;
      border-radius: 50%;
    }
}
</style>