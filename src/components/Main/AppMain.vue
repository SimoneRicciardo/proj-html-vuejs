<template>
  <div>
    <SectionArtistCoaching/>
    <SectionPaintings/>
    <SectionArticles/>
    <SectionEvents/>
  </div>
</template>

<script>
import SectionArtistCoaching from "./section1/SectionArtistCoaching.vue";
import SectionPaintings from "./section2/SectionPaintings.vue";
import SectionArticles from "./section3/SectionArticles.vue";
import SectionEvents from "./section4/sectionEvents.vue";
export default {
    name: "AppMain",
    components: {
    SectionArtistCoaching,
    SectionPaintings,
    SectionArticles,
    SectionEvents
}
}
</script>

<style lang="scss">

</style>