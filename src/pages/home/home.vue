<template>
  <div>
    <home-header></home-header>
    <home-search></home-search>
    <home-banner></home-banner>
    <home-category :categories="categories"></home-category>
  </div>
</template>

<script>
import axios from 'axios'
import HomeHeader from './components/header.vue'
import HomeSearch from './components/search.vue'
import HomeBanner from './components/banner.vue'
import HomeCategory from './components/category.vue'
export default {
  name: 'Home',
  components: {
    'home-header': HomeHeader,
    'home-search': HomeSearch,
    'home-banner': HomeBanner,
    'home-category': HomeCategory
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
