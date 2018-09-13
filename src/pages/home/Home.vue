<template>
  <div>
    <nav-content></nav-content>
    <home-header></home-header>
    <home-banner></home-banner>
    <home-article></home-article>
  </div>
</template>

<script>
import navContent from '../components/nav'
import homeHeader from './components/Header'
import homeBanner from './components/Banner'
import homeArticle from './components/Article'
export default {
  name: 'Home',
  components: {
    homeHeader,
    homeBanner,
    navContent,
    homeArticle
  }
}
</script>
<style scoped>
</style>
