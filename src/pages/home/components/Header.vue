<template>
    <div>
      <div class="navBar">
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
}
</script>
<style scoped lang="less">
  .navBar{
    position:fixed;
    min-height:50px;
    margin-bottom:20px;
    width:100%;
    z-index: 10;
    background-color:rgba(255,255,255,0.6);
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
        left:30px;
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
