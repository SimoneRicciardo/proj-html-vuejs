<template>
  <div class="container">
    <div class="container-hero">
      <img class="img-hero-back img-01" src="@/images/artist-shape-03.png" alt="">
      <img class="img-hero-back img-04" src="@/images/artist-hero-image-03-204x300.png" alt="">
      <img class="img-hero-back img-03" src="@/images/artist-hero-image-02-232x300.jpg" alt="">
      <img class="img-hero-back img-02" src="@/images/artist-hero-image-01.jpg" alt="">
      <img class="img-hero-back img-05" src="@/images/artist-hero-image-04-235x300.jpg" alt="">
      <img class="img-hero-back img-06" src="@/images/artist-shape-05.png" alt="">
      <img class="img-hero-back img-07" src="@/images/artist-shape-04-127x300.png" alt="">
      <img class="img-hero-back img-08" src="@/images/artist-shape-03-201x300.png" alt="">
  
      <div class="info-hero">
        <span>
          Hello,Im Matin
        </span> 
        <h1>
          Artist Coaching And Mentoring Might Be for You.
        </h1>
        <button class="btn btn-orange">Get started today</button>
      </div>
    </div>
    
  </div>
</template>

<script>
export default {
    name: 'HeroSection'
}
</script>

<style lang="scss">

.container{
  background: url(@/images/artist-shape-01.png), url(@/images/artist-shape-02-768x415.png),  rgb(251, 249, 246);
  background-repeat: no-repeat;
  background-position-x: right, 0;
  height: 800px;
}
.container-hero{
    width: 1200px;
    margin: 0 auto;

    .img-hero-back{
      position: relative;
    }

    .img-01{
      top: 186px;
      left: -640px;
      
    }
    .img-02{    
      top: 227px;
      left: -1281px;
    }
    .img-03{
      top: 19px;
      left: -865px;
    }
    .img-04{
      top: 236px;
      left: -554px;
    }
    .img-05{
      top: -116px;
      left: 1360px;
      z-index: 1;
    }
    .img-06{
      top: -93px;
      left: 1120px;
    }
    .img-07{
      top: -295px;
      left: 958px;
    }
    .img-08{
      top: -80px;
      left: 606px;
    }

    .info-hero{
      display: flex;
      flex-direction: column;
      align-items: center;
      position: relative;
      bottom: 420px;

      h1{
        text-align: center;
        width: 745px;
        padding: 30px 0;
        font-size: 50px;
      }
    }
}
</style>