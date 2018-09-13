<template>
    <div>
      <div class="navBar" ref="navBar">
        <div class="navHeader">
          <div class="container">
            <div class="logo">
              <a href="">
                <img src="../../../assets/img/nice.png" alt="">
              </a>
            </div>
            <ul class="navUl">
              <li><a href="#">一季花开花落</a></li>
              <li><a href="#">git</a></li>
              <li><a href="#">关于我</a></li>
              <li><a href="#">Welcome!</a></li>
            </ul>
          </div>
        </div>
      </div>
    </div>
</template>
<script>
export default {
  name: 'homeHeader'
  // mounted () {
  //   const that = this
  //   window.onscroll = function () {
  //     let t = document.documentElement.scrollTop || document.body.scrollTop
  //     let vh = 1
  //     const tvh = t + vh
  //     if (tvh > t) {
  //       that.$refs.navBar.style.top = '-60px'
  //       that.$refs.navBar.style.opacity = 0
  //     } else {
  //       that.$refs.navBar.style.top = '0'
  //       that.$refs.navBar.style.opacity = 1
  //     }
  //   }
  // }
}
</script>
<style scoped lang="less">
  .navBar{
    position:fixed;
    min-height:50px;
    margin-bottom:20px;
    width:100%;
    z-index: 10;
    top:0;
    left:0;
    opacity: 1;
    background-color:rgba(255,255,255,0.8);
    /*-webkit-transition: opacity,top 500ms linear;*/
    /*transition: opacity,top 500ms linear;*/
    .navHeader{
      background-color:transparent;
      -webkit-transition: background-color 400ms linear;
      transition: background-color 400ms linear;
      border:none;
      .logo{
        position:absolute;
        display: block;
        top:50%;
        margin-top:-15px;
        left:15px;
        a{
          display: block;
          img{
            width:30px;
          }
        }
      }
      .navUl{
        display: block;
        width:100%;
        height:60px;
        text-align: center;
        line-height:60px;
        li{
          display: inline-block;
          a{
            display: block;
            padding:0 10px;
            border-right:1px solid #aaa;
            font-size:12px;
            line-height:14px;

          }
        }
        li:last-child{
          a{
            border:none;
          }
        }
      }
    }
  }
</style>
