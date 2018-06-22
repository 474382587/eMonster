<template>
  <div class="featured">
    <div class="featured-item">
      <p class="title">title</p>
      <p class="description">description</p>
      <div class="more-info">item-link &gt;</div>
      <img class="item-img" src="static/featured1.png" alt="">
    </div>
    <div class="featured-item right">
      <p class="title">title</p>
      <p class="description">description</p>
      <div class="more-info">
        <span class="number">number</span>
        <span class="item-link"> item-link &gt;</span>
      </div>
      <img class="item-img" src="static/featured2.png" alt="">
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeFeaured'
}
</script>

<style lang="stylus" scoped>
.featured
  display: flex;
  justify-content: space-between;
  padding: 0 .2rem;
  .featured-item:first-child
    margin-right .1rem
  .featured-item
    background-color #f6f6f6
    padding 0.2rem .3rem
    height 2.4rem
    flex: 1;
    position relative
    .title
      font-weight 600
      font-size .42rem
      height .46rem
      height .46rem
    .description
      line-height .32rem
      height .32rem
      font-size .28rem
      color #666
    .item-img
      position absolute
      bottom -.14rem
      right 0
      display block
      width 2.4rem
    .more-info
      font-size .32rem
      line-height .52rem
      height .52rem
      color #af8260
      .number
        color red
      .item-link
        color #000
.right
  .title
    color red
</style>
