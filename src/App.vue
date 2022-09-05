<template>
  <div id="app">
    <AppHeader/>
    <AppMain/>
    <AppFooter/>
  </div>
</template>

<script>
import AppHeader from './components/Header/AppHeader.vue';
import AppMain from './components/Main/AppMain.vue';
import AppFooter from './components/Footer/AppFooter.vue';

export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
    AppFooter
}
}
</script>

<style lang="scss">
@import './styleSCSS/genericRule.scss';
@import '~@fortawesome/fontawesome-free/css/all.css'

</style>
