<template>
  <div>
    <home-header></home-header>
    <home-banner></home-banner>
  </div>
</template>

<script>
import homeHeader from './components/Header'
import homeBanner from './components/Banner'
export default {
  name: 'Home',
  components: {
    homeHeader,
    homeBanner
  }
}
</script>
<style scoped>
</style>
