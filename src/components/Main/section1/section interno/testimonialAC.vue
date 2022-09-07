<template>
  <div>
    <div class="title-testimonial">
      <span>
        Testimonial
      </span> 
      <h2>
        Why do people love me?
      </h2>
    </div>

    <div class="card-testimonial">
      <div v-for="(testimonial, index) in cardTestimonialList" :key="index" class="testimonial">
        <h4>{{testimonial.title}}</h4>
        <p>{{testimonial.description}}</p>
        <div class="img-name-card">
          <img :src='"@/images/artist-testimonial-avatar-" + testimonial.img + ".jpg"' alt="">
          <div>
              <h4>{{testimonial.name}}</h4>
              <p>{{testimonial.profession}}</p>
          </div>
        </div>

      </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'testimonialAC',
    data() {
        return {
            cardTestimonialList: [
                {
                    img: "01",
                    title: "High level of efficiency and scientific teaching methods",
                    description: "i am ffree to learn at my own pace, follow my own sschedule and choose the subject i want to learn from the syllabuss. Great study portal for people like me.",
                    name: "Mina Hollace",
                    profession: "/Freelancer"
                },
                {
                    img: "02",
                    title: "High level of efficiency and scientific teaching methods",
                    description: "i am ffree to learn at my own pace, follow my own sschedule and choose the subject i want to learn from the syllabuss. Great study portal for people like me.",
                    name: "Mina Hollace",
                    profession: "/Freelancer"
                },
                {
                    img: "03",
                    title: "High level of efficiency and scientific teaching methods",
                    description: "i am ffree to learn at my own pace, follow my own sschedule and choose the subject i want to learn from the syllabuss. Great study portal for people like me.",
                    name: "Mina Hollace",
                    profession: "/Freelancer"
                },
            ]
        };
    }
}
</script>

<style lang="scss">
.title-testimonial{
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
  margin: 110px 0;

  h2{
    padding-top:10px;
  }
}
.card-testimonial{

  display: flex;
  justify-content: space-around;
  height: 300px;
  padding-bottom: 100px;

  .testimonial{
    display: flex;
    flex-direction: column;
    justify-content: space-around;
    width: 450px;
    padding: 25px;
    background-color: #fff;
  }

  .img-name-card{
    display: flex;
    align-items: center;
    
    div{
        padding: 0 15px;
        h4{
            padding-bottom: 10px ;
        }
    }
  }

  img{
    height: 70px;
    border-radius: 50%;
  }
}
</style>