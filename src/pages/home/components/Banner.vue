<template>
  <div>
    <div class="homeBanner" ref="heightBlack">
      <div class="container-fluid bannerBg element-img">
        <div class="bannerContent"></div>
      </div>
    </div>
    <!--<div class="heightBlack" ref="heightBlack"></div>-->
  </div>
</template>
<script>
export default {
  name: 'homeBanner',
  mounted () {
    const height = document.body.offsetHeight
    this.$refs.heightBlack.style.height = height + 'px'
  }
}
</script>

<style scoped lang="less">
  .homeBanner{
    position:relative;
    top:0;
    left:0;
    width:100%;
    /*height:100vh;*/
    .bannerBg{
      background:url(../../../assets/img/bg1.jpeg) no-repeat center center fixed;
      background-size:cover;
      .bannerContent{}
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
