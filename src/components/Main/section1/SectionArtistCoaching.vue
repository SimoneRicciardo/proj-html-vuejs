<template>
  <!-- ac = ArtistCoaching  per identificare la sezione -->
<div>

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