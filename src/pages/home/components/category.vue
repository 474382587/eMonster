<template>
  <div class="categories">
    <swiper ref="mySwiper ">
    <swiper-slide v-for="(item,index) in separate" :key="index">
      <div class="category" v-for="category in item" :key="category.id">
        <img class="cate-img" :src="category.imgUrl" alt="category.id">
        <p class="title">
          {{category.name}}
        </p>
      </div>
    </swiper-slide>
    <div class="swiper-pagination"  slot="pagination"></div>
  </swiper>
  </div>
</template>
<script>
export default {
  name: 'HomeCategory',
  props: {
    categories: Array
  },
  computed: {
    separate () {
      let result = []
      for (let i = 0; i < this.categories.length; i += 10) {
        result.push(this.categories.slice(i, i + 10))
      }
      return result
    }
  }
}
</script>

<style lang="stylus" scoped>
.categories {
  padding: 0.2rem;

  .category {
    width: 20%;
    float: left;
    text-align: center;

    .cate-img {
      width: 0.9rem;
    }

    .title {
      margin-top: 0.16rem;
      font-size: 0.24rem;
      white-space: nowrap;
      text-overflow: ellipsis;
      overflow: hidden;
    }
  }
}
</style>
