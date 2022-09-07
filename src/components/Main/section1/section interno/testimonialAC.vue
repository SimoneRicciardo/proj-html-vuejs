<template>
  <div>
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
                {
                    img: "04",
                    title: "High level of efficiency and scientific teaching methods",
                    description: "i am ffree to learn at my own pace, follow my own sschedule and choose the subject i want to learn from the syllabuss. Great study portal for people like me.",
                    name: "Mina Hollace",
                    profession: "/Freelancer"
                }
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