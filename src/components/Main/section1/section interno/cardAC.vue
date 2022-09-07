<template>
  <div>
    <div class="ac-card">
        <div v-for="(skils, index) in skilsList" :key="index">
            <img :src='"@/images/artist-box-image-" + skils.img + ".png"' alt="">
            <span>{{skils.title}}</span>
            <p>{{skils.description}}</p>
        </div> 
    </div>

    <div class="ac-info">
        <div class="info-sx">
            <img src="@/images/artist-quote-icon.png" alt="">
            <h1>I coach and mentor visual artist, like you, to Create Like You Mean It</h1>
            <span>Martin Garrix</span>
        </div>

        <div class="info-dx">
            <p>As a coach and mentor, my ultimate goal is to motivate visual artist toward inspired action, I help you get you back on track to being the productive, creative, meaningful and authentic artist you truly want to be. I support artist in crafting and living a creative life as well as feeling good about themselves and thei art.</p>
            <span>As an artist and an educator for nearly 30 years, i understand what it takess to create.</span>
            <div>
                <button class="btn btn-light-orange">Get started today</button>
            </div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    name: 'CardAC',

    data(){
        return{
            skilsList: [
                {
                    img: "01",
                    title: "Online Coures",
                    description: "Online art coaching now offers you a very powerful way to redesing your artist mind."
                },
                {
                    img: "02",
                    title: "One to One",
                    description: "Getting the necessary clarity about the current state to help you improve your ability."
                },
                {
                    img: "03",
                    title: "Anywhere",
                    description: "Access to valuable and portable program which allow you to step and live anywhere you want."
                },
                {
                    img: "04",
                    title: "On Time",
                    description: "Punctualy i our priority beacause it`s an essential to assess a program quality."
                }
            ]
        }
    }
}
</script>

<style lang="scss">
.ac-card{
display: flex;
justify-content: center;
margin: 100px 0;

    span{
        font-weight: bold;
        padding: 15px 0;
    }

    p{
        font-size: 15px;
        color: rgb(106, 106, 107);
        font-weight: 500;
    }

    div{
        width: calc(100%/4);
        display: flex;
        flex-direction: column;
        padding: 0  25px;

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
        
        h1{
            width: 360px;
            font-weight: 700;
            padding: 25px 0
        }
    
        img{
        width: 30px;
        }
    }
    .info-dx{
    width: 500px;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    justify-content: flex-end;
    font-size: 15px;
    color: rgb(106, 106, 107);
    font-weight: 500;
        span{
            padding:15px 0;
        }
    }
}
</style>