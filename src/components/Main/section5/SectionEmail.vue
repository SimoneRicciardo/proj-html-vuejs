<template>
  <div class="container-email">
    <span>Newsletter to get in touch</span>
    <input type="email" placeholder="Your e-mail" />

  </div>
</template>

<script>
export default {
    name: 'SectionEmail', 
}
</script>

<style lang="scss">
.container-email{
    text-align: center;
    margin-top:100px ;
    padding:50px 0;
    background-color: rgb(36, 65, 134);
    background-image: url(@/images/artist-shape-color-paint-bottom-right-300x153.png), url(@/images/artist-shape-color-paint-top-left.png);
    background-repeat: no-repeat;
    background-position-x: right, 0;

    span{
        padding: 0 25px;
    }
}
</style>