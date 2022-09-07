<template>
  <div>
    <SectionArtistCoaching/>
    <SectionPaintings/>
    <SectionArticles/>
    <SectionEvents/>
    <SectionEmail/>
  </div>
</template>

<script>
import SectionArtistCoaching from "./section1/SectionArtistCoaching.vue";
import SectionPaintings from "./section2/SectionPaintings.vue";
import SectionArticles from "./section3/SectionArticles.vue";
import SectionEvents from "./section4/sectionEvents.vue";
import SectionEmail from "./section5/SectionEmail.vue";
export default {
    name: "AppMain",
    components: {
    SectionArtistCoaching,
    SectionPaintings,
    SectionArticles,
    SectionEvents,
    SectionEmail
}
}
</script>

<style lang="scss">

</style>