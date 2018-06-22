<template>
  <div class="nav-bar">
    <div class="nav-item active">
      <img class="symbol" src="static/temp.png" alt="">
      Home
    </div>
    <div class="nav-item">
      <img class="symbol" src="static/temp.png" alt="">
      Discover
    </div>
    <div class="nav-item">
      <img class="symbol" src="static/temp.png" alt="">
      Order
    </div>
    <div class="nav-item">
      <img class="symbol" src="static/temp.png" alt="">
      Mine
    </div>
  </div>
</template>

<script>
export default {
  name: 'BottomNav'
}
</script>

<style lang="stylus" scoped>
.nav-bar
  position fixed
  bottom 0
  left 0
  right 0
  z-index 999
  background-color #ffffff
  display flex
  justify-content space-around
  box-shadow 0 0 .6rem .1rem #e3e3e3
  padding .12rem 0
  .nav-item
    flex 1
    display flex
    flex-direction column
    text-align center
    align-items center
    .symbol
      width 40%
  .nav-item.active
    color #0089dc
</style>
