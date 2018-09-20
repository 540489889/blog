<template>
  <div>
    <div class="footer">
      <div class="container">
        <div class="copy">
          <p>
            © 2014 -2018, Content By Kieran. All Rights Reserved.
          </p>
          <p>Theme By <a style="color: #767D84">Kieran</a></p>
        </div>
        <div class="social">
          <ul>
            <li><a href="https://github.com/SuperKieran" title="Github" target="_blank"><i class="icon-github"></i></a></li>
            <li><a href="https://twitter.com/1tsKieran" title="Twitter" target="_blank"><i class="icon-twitter"></i></a></li>
            <li><a href="http://weibo.com/taokailun" title="Sina-Weibo" target="_blank"><i class="icon-sina-weibo"></i></a></li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'homeFooter'
}
</script>

<style scoped lang="less">
  .footer{
    padding: 4% 0;
    background: #151515;
    z-index: 9;
    position: relative;
    overflow: hidden;
    .copy{
      float: left;
      margin-top: 5px;
      p{
        font-size: 12px;
        color: #767D84;
        margin-top:5px;
      }
    }
    .social{
      float: right;
      margin-top: 5px;
      ul{
        li{
          background: none;
          display: inline-block;
        }
      }
    }
  }
</style>
