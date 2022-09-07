<template>
  <div class="container-email">
    <h2>Newsletter to get in touch</h2>
    <input type="text" placeholder="Your e-mail" />
    <a href=""><i class="fas fa-arrow-right"></i></a>
  </div>
</template>

<script>
export default {
    name: 'SectionEmail', 
}
</script>

<style lang="scss">
.container-email{
    display: flex;
    justify-content: center;
    padding:50px 0;
    background-color: rgb(36, 65, 134);
    background-image: url(@/images/artist-shape-color-paint-bottom-right-300x153.png), 
                      url(@/images/artist-shape-color-paint-top-left.png);
    background-repeat: no-repeat;
    background-position-x: right, 0;

    h2{
      margin-right: 100px;
        text-align: end;
        width: 250px;
        padding: 0 25px;
        color: white;
    }
    input{
      width: 500px;
      border: none;
      border-bottom: 2px solid white;
      background-color: rgb(36, 65, 134);
      color: white;
    }
    i{
      position: relative;
      top: 20px;
      right: 20px;
      font-size: 20px;
      color: white;
    }
}
</style>