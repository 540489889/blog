<template>
  <div>
    <div class="homeBanner">
      <div class="container-fluid bannerBg element-img"></div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'homeBanner'
}
</script>

<style scoped lang="less">
  .homeBanner{
    position:fixed;
    top:0;
    left:0;
    width:100%;
    height:100%;
    .bannerBg{
      background:url(../../../assets/img/bg.jpg) no-repeat center center fixed;
      background-size:cover;
    }
    .element-img{
      -webkit-background-size: cover;
      -moz-background-size: cover;
      -o-background-size: cover;
      background-size: cover;
      background-position: center center;
      background-repeat: no-repeat;
      height: 100%;
      position: relative;
      z-index: 8;
      background-repeat: no-repeat;
    }
  }
</style>
