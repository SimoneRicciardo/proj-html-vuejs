<template>
  <div class="container-hero">
    <img src="@/images/artist-shape-03.png" alt="">
    <img src="@/images/artist-hero-image-01.jpg" alt="">
    <img src="@/images/artist-hero-image-02-232x300.jpg" alt="">
    <img src="@/images/artist-hero-image-03-204x300.png" alt="">
    <img src="@/images/artist-hero-image-04-235x300.jpg" alt="">
    <img src="@/images/artist-shape-05.png" alt="">
    <img src="@/images/artist-shape-04-127x300.png" alt="">
    <img src="@/images/artist-shape-03-201x300.png" alt="">

    <div class="info-hero">
      <span>
        Hello,Im Matin
      </span> 
      <span>
        Artist Coaching And Mentoring Might Be for You
      </span>
      <button>Get started today</button>
    </div>
    
  </div>
</template>

<script>
export default {
    name: 'HeroSection'
}
</script>

<style lang="scss">
.container-hero{
  background: url(@/images/artist-shape-01.png), url(@/images/artist-shape-02-768x415.png),  rgb(251, 249, 246);
  background-repeat: no-repeat;
  background-position-x: right, 0;

    .info-hero{
      display: flex;
      flex-direction: column;
      align-items: center;
    }
}
</style>