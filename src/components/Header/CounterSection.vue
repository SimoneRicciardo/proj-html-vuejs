<template>
  <div class="container-count">
    <p>Starts TOMORROW! Oru biggest eventof the year....</p>
    <div>icona+ 00:00:00:00</div>
    <button>Get ticket</button>
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

    div{
      padding: 0 35px;
    }
}
</style>