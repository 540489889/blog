<template>
  <div>
    <nav-content></nav-content>
    <home-header></home-header>
    <home-banner></home-banner>
    <home-article></home-article>
    <statement></statement>
    <home-footer></home-footer>
  </div>
</template>

<script>
import navContent from '../components/nav'
import homeHeader from './components/Header'
import homeFooter from './components/Footer'
import homeBanner from './components/Banner'
import homeArticle from './components/Article'
import statement from './components/Statement'
export default {
  name: 'Home',
  components: {
    homeHeader,
    homeBanner,
    navContent,
    homeArticle,
    homeFooter,
    statement
  }
}
</script>
<style scoped>
</style>
