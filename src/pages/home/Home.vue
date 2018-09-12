<template>
  <div>
    <nav-content></nav-content>
    <home-header></home-header>
    <home-banner></home-banner>
  </div>
</template>

<script>
import navContent from '../components/nav'
import homeHeader from './components/Header'
import homeBanner from './components/Banner'
export default {
  name: 'Home',
  components: {
    homeHeader,
    homeBanner,
    navContent
  }
}
</script>
<style scoped>
</style>
