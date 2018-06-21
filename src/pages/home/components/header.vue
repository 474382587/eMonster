<template>
  <div class="header">
    <div class="header-city">
      <span class="header-icon iconfont">&#xe640;</span>
      <span class="city-name">City Name</span>
      <span class="down-arrow iconfont">&#xe617;</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeHeader'
}
</script>

<style lang="stylus" scoped>
.header
  background-image linear-gradient(90deg,#0af,#0085ff)
  color #ffffff
  padding  .2rem .28rem 0
  .header-city
    height .6rem
    line-height .6rem
    font-size .36rem
    max-width 4rem
    .city-name
      margin-right 0.2rem
    .down-arrow
      font-size .24rem
</style>
