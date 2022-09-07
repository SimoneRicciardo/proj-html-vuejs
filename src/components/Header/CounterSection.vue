<template>
  <div class="container-count">
    <p>Starts TOMORROW! Oru biggest eventof the year....</p>
    <div><i class="fa-regular fa-clock"></i> 00:00:00:00</div>
    <button class="btn-counter btn-orange">Get ticket</button>
  </div>
</template>

<script>
export default {
    name:'CounterSection'
}
</script>

<style lang="scss">
.container-count{
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: rgb(235, 235, 235);
  height: 50px;

    p{
      color: rgb(157, 157, 157);
      font-size: 14px;
    }

    div{
      padding: 0 35px;
    }

    .btn-counter{
      padding: 6px 25px;
      border-radius: 5px;
      border: none;
      font-weight: 700;
    }
}
</style>