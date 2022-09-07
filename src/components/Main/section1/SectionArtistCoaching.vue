<template>
  <!-- ac = ArtistCoaching  per identificare la sezione -->
<div class="container-ac">

  <div class="container-section-ac">

    <div class="info-hero text-center">
      <span>
        Artist coaching
      </span> 
      <h2>
        I understand what it takes to create. I can help you with
      </h2>
    </div> 

    <CardAC/>

  </div>
  
  <ImgAC/>

  <TestimonialAC/>

</div>
</template>

<script>
import CardAC from './section interno/cardAC.vue';
import ImgAC from './section interno/imgAC.vue';
import TestimonialAC from './section interno/testimonialAC.vue';
export default {
    name: "SectionArtistCoaching",
    components: {
    CardAC,
    ImgAC,
    TestimonialAC
}
}
</script>

<style  lang="scss">
 
.container-ac{
  background: url(@/images/artist-shape-01-600x577.png), 
              url(@/images/maxcoach-shape-14-1536x343.png) -8px 95px,
              url(@/images/maxcoach-shape-13-150x150.png) 2315px 60px,
              url(@/images/artist-shape-05.png) 500px,
              url(@/images/maxcoach-shape-12-150x150.png) 713px 785px,
              url(@/images/maxcoach-shape-12-150x150.png) 1685px 1245px,
              url(@/images/artist-shape-01-600x577.png) -275px 961px;

  background-size:500px, 2560px 300px, 250px 250px,600px, 200px, 150px, 2969px 1442px;
  background-repeat: no-repeat;
}

.container-section-ac{
  width: 1070px;
  margin: 0 auto;

  .info-hero{
      margin: 100px 0;
      h2{
        padding: 13px 0;
      }
    }
}
</style>

<!--  -->