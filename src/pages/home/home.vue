<template>
  <div class="home">
    <home-header></home-header>
    <home-search></home-search>
    <home-banner></home-banner>
    <home-category :categories="categories"></home-category>
    <home-featured></home-featured>
    <home-recommend></home-recommend>
    <bottom-nav></bottom-nav>
  </div>
</template>

<script>
import axios from 'axios'
import HomeHeader from './components/header.vue'
import HomeSearch from './components/search.vue'
import HomeBanner from './components/banner.vue'
import HomeCategory from './components/category.vue'
import HomeFeatured from './components/featured.vue'
import HomeRecommend from './components/recommend.vue'
import BottomNav from '@/components/bottom-nav.vue'
export default {
  name: 'Home',
  components: {
    'home-header': HomeHeader,
    'home-search': HomeSearch,
    'home-banner': HomeBanner,
    'home-category': HomeCategory,
    'home-featured': HomeFeatured,
    'home-recommend': HomeRecommend,
    'bottom-nav': BottomNav
  },
  data () {
    return {
      categories: []
    }
  },
  mounted () {
    axios.get('static/mock/category.json').then(res => {
      const data = res.data
      console.log(data)
      this.categories = data.category
    })
  }
}
</script>

<style lang="stylus" scoped>
</style>
