<template>
  <div>
    <div class="article" id="article">
      <div class="container">
        <div class="row">
          <div class="col-md-8 offset-md-2">
            <div class="row">
              <div class="col-md-4">
                <h3 class="article-title">CSS 样式防御</h3>
                <p class="article-time">2018-08-25 | CSS3, iframe, Shadow DOM</p>
              </div>
              <div class="col-md-8">
                <div class="article-info">概念 / 起因什么是样式防御？顾名思义，就是保护你写的样式最后是你想展现的样子。一般样式被破坏多发生于第三方应用编程中，当编写的组件被应用于第三方网站中，组件的样式经常会被网站本身的样式影响而破坏了它本来想展现的样子。 为什么会研究这个东西呢？因为有一天，我引用的第三方代码的 CSS 被我网站上的 CSS 影响了。于是，我噼里啪啦赶紧把第三方的样式又给“强调“了一遍。搞完一想，不对啊，这特么应该是第三方自己没做好对自己 CSS 代</div>
                <p class="pull-right text-right readMore">
                  <a href="">Read More...</a>
                </p>
              </div>
            </div>
            <div class="nogutter"></div>
          </div>
        </div>
        <div class="row">
          <div class="col-md-8 offset-md-2">
            <div class="row">
              <div class="col-md-4">
                <h3 class="article-title">前端也需要了解的 JSONP 安全</h3>
                <p class="article-time">2018-08-10 | JavaScript, Security, JSONP</p>
              </div>
              <div class="col-md-8">
                <div class="article-info">什么是 JSONP（JSON with Padding）？What? 你还不知道 JSONP 是什么？赶紧去补补吧，我就不多讲了。补个百度百科链接先，https://baike.baidu.com/item/jsonp/493658 会有哪些安全隐患？怎么防范？我们假设有这样一个场景一我登录了 www.qq.com，QQ 为了给第三方提供服务，可能会有这样的 jsonp 接口，www.qq.com/getUserInfo?callba</div>
                <p class="pull-right text-right readMore">
                  <a href="">Read More...</a>
                </p>
              </div>
            </div>
            <div class="nogutter"></div>
          </div>
        </div>
        <div class="row">
          <div class="col-md-8 offset-md-2">
            <div class="row">
              <div class="col-md-4">
                <h3 class="article-title">南北湖 / 奕仙城 / 未完成的一日一夜游小记</h3>
                <p class="article-time">2018-01-06 | 南北湖, 奕仙城, Travel</p>
              </div>
              <div class="col-md-8">
                <div class="article-info">先来段正规的介绍12345南北湖，浙江省第一批省级风景名胜区、国家AAAA级旅游景区、浙江十大“最佳休闲度假胜地”之一。南北湖，山有层次，水有曲折，海有奇景，村有故事，是我国唯一融山、海、湖、村为一体的全景度假地，依托山海湖·村特色资源，提供多种主题度假方式，感受完美全景度假生活。门票：80元预订：60元海盐本地居民凭 330424 开头的身份证可以办理南北湖旅游年卡，无限次进入南北湖，20元/年年卡办理公众号：nanbeihuly 首</div>
                <p class="pull-right text-right readMore">
                  <a href="">Read More...</a>
                </p>
              </div>
            </div>
            <div class="nogutter"></div>
          </div>
        </div>
        <div class="row">
          <div class="col-md-8 offset-md-2">
            <div class="row">
              <div class="col-md-4">
                <h3 class="article-title">CSS 样式防御</h3>
                <p class="article-time">2018-08-25 | CSS3, iframe, Shadow DOM</p>
              </div>
              <div class="col-md-8">
                <div class="article-info">概念 / 起因什么是样式防御？顾名思义，就是保护你写的样式最后是你想展现的样子。一般样式被破坏多发生于第三方应用编程中，当编写的组件被应用于第三方网站中，组件的样式经常会被网站本身的样式影响而破坏了它本来想展现的样子。 为什么会研究这个东西呢？因为有一天，我引用的第三方代码的 CSS 被我网站上的 CSS 影响了。于是，我噼里啪啦赶紧把第三方的样式又给“强调“了一遍。搞完一想，不对啊，这特么应该是第三方自己没做好对自己 CSS 代</div>
                <p class="pull-right text-right readMore">
                  <a href="">Read More...</a>
                </p>
              </div>
            </div>
            <div class="nogutter"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'homeArticle'
}
</script>

<style scoped lang="less">
  .article{
    background-color:white;
    position:relative;
    padding-top:60px;
    z-index: 4;
    .article-title{
      font-style: normal;
      font-weight: 400;
      line-height: 37px;
      font-size: 20px;
      margin-top: 0;
    }
    .article-text{
      color:#666;
    }
    .article-info{
      line-height:1.8;
      color:#666;
      margin-bottom:10px;
    }
    .readMore a{
      font-size: 12px;
      color: gray;
      padding-top: 2px;
      padding-bottom: 2px;
      padding-left: 10px;
      padding-right: 10px;
      border: 1px solid gray;
      border-radius: 20px;
    }
    .nogutter{
      height: 0;
      -webkit-box-sizing: content-box;
      -moz-box-sizing: content-box;
      box-sizing: content-box;
      border: 0;
      border-top: 1px solid #eee;
      margin-top: 40px;
      margin-bottom: 40px;
    }
  }
</style>
