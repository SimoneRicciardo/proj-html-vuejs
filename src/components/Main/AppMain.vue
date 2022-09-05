<template>
  <div>
    <SectionArtistCoaching/>
    <SectionPaintings/>
  </div>
</template>

<script>
import SectionArtistCoaching from "./section1/SectionArtistCoaching.vue";
import SectionPaintings from "./ssection2/SectionPaintings.vue";
export default {
    name: "AppMain",
    components: { 
      SectionArtistCoaching, 
      SectionPaintings }
}
</script>

<style lang="scss">

</style>