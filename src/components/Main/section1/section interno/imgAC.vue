<template>
    <div class="ac-img">
      <img src="@/images/artist-video-poster.jpg" alt="">
      <a href="" class="ac-play">
        <img src="@/images/icon-youtube-play.png" alt="">
      </a>
    </div>
</template>

<script>
export default {
    name: 'imgAC',
}
</script>

<style lang="scss">
.ac-img{
display: flex;
justify-content: center;
margin-top: 110px;
position: relative;

    .ac-play{
        position: absolute;
        top: 50%;
    }
}

</style>