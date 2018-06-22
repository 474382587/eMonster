<template>
  <div class="recommend">
    <div class="title"><span class="content">Recommend</span></div>
    <div class="item">
      <div class="detail">
        <div class="detail-logo">
          <img src="//fuss10.elemecdn.com/c/62/5d1390cdc0f754fcf691128684986jpeg.jpeg" alt="logo">
        </div>
        <div class="detail-description">
          <div class="detai-title">
            <span class="content">Cooking Master (Vancouver)</span>
            <span class="support">G</span>
          </div>
          <div class="rating">
            <p class="sale">
              <img class="rating-img" src="static/rating.svg" alt="">
              500 sold in May
            </p>
            <p class="extra-info">Express</p>
          </div>
          <div class="delivery">
            <div class="left"><span class="requirement">Over $25</span> | <span class="charge">$3</span></div>
            <div class="right">
              <span class="distance">355m</span>
              |
              <span class="time">25min</span>
            </div>
          </div>
        </div>
      </div>
      <div class="promo">
        <div class="activity">
          <div class="promo-fisrt">
            <span class="icon">1st</span>
            Promo1
          </div>
          <div class="promo-second">
            <span class="icon">2nd</span>
            promo2
          </div>
        </div>
        <div class="more-promo">5 more <img src="static/down-arrow.svg" alt="down"></div>
      </div>
    </div>
    <div class="item">
      <div class="detail">
        <div class="detail-logo">
          <img src="//fuss10.elemecdn.com/c/62/5d1390cdc0f754fcf691128684986jpeg.jpeg" alt="logo">
        </div>
        <div class="detail-description">
          <div class="detai-title">
            <span class="content">Cooking Master (Vancouver)</span>
            <span class="support">G</span>
          </div>
          <div class="rating">
            <p class="sale">
              <img class="rating-img" src="static/rating.svg" alt="">
              500 sold in May
            </p>
            <p class="extra-info">Express</p>
          </div>
          <div class="delivery">
            <div class="left"><span class="requirement">Over $25</span> | <span class="charge">$3</span></div>
            <div class="right">
              <span class="distance">355m</span>
              |
              <span class="time">25min</span>
            </div>
          </div>
        </div>
      </div>
      <div class="promo">
        <div class="activity">
          <div class="promo-fisrt">
            <span class="icon">1st</span>
            Promo1
          </div>
          <div class="promo-second">
            <span class="icon">2nd</span>
            promo2
          </div>
        </div>
        <div class="more-promo">5 more <img src="static/down-arrow.svg" alt="down"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeRecommend'
}
</script>

<style lang="stylus" scoped>
.title
  text-align center
  line-height .56rem
  height .56rem
  margin .2rem
  .content
    font-size .32rem
    position relative
    &::before
      position absolute
      top 50%
      right calc(100% + 0.2rem)
      content ""
      display block
      width .4rem
      border 1px solid #666
    &::after
      position absolute
      top 50%
      left calc(100% + 0.2rem)
      content ""
      display block
      width .4rem
      border 1px solid #666
.item
  display flex
  flex-direction column
  justify-content flex-start
  margin .2rem 0 .4rem
  padding 0 .2rem
  .detail
    display flex
    justify-content space-between
    .detail-logo
      flex none
      img
        width 1.3rem
    .detail-description
      flex 1
      display flex
      flex-direction column
      justify-content space-between
      padding .04rem .2rem
      .detai-title
        font-size .3rem
        text-align left
        justify-content space-between
        display flex
        align-items center
        .content
          &::before
            flex 0
            line-height normal
            font-size .24rem
            padding .04rem .06rem
            margin-right .1rem
            color #6f3f15
            content: 'Brand'
            background-image linear-gradient(-139deg,#fff100,#ffe339)
        .support
          color #666
      .rating
        .rating-img
          height .24rem
          margin-right .1rem
        display flex
        align-items center
        justify-content space-between
        color #666
        .extra-info
          padding .02rem
          color #ffffff
          background-image linear-gradient(45deg,#0085ff,#0af)
      .delivery
        display flex
        justify-content space-between
        color #666
        .right
          color #888
  .promo
    margin-top .2rem
    padding .1rem .2rem .1rem 1.5rem
    display flex
    justify-content space-between
    .more-promo
      color #888
      img
        width .2rem
    .promo-fisrt
      margin-bottom .2rem
      .icon
        background-color rgb(112, 188, 70)
        color #ffffff
        padding .02rem .04rem
    .promo-second
      .icon
        background-color rgb(240, 115, 115)
        color #ffffff
        padding .02rem .04rem
</style>
