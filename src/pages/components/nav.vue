<template>
    <div>
      <div class="pos-f-t" style="display: block">
        <div ref="menuContent" id="navbarToggleExternalContent">
          <div class="sb-close text-right" @click="closeMenu"><img src="../../assets/img/close.png" alt=""></div>
          <div class="p-4">
            <div class="list-group">
              <a href="#" class="list-group-item list-group-item-action">Home</a>
              <a data-toggle="collapse" data-target="#demo" aria-expanded="true" aria-controls="collapseOne" class="list-group-item list-group-item-action dropdown">Tags</a>
              <ul id="demo" class="collapse">
                <li><a class="list-group-item list-group-item-action">php</a></li>
                <li><a class="list-group-item list-group-item-action">javascript</a></li>
                <li><a class="list-group-item list-group-item-action">html</a></li>
                <li><a class="list-group-item list-group-item-action">css</a></li>
              </ul>
              <a href="#" class="list-group-item list-group-item-action ">Link</a>
              <a href="#" class="list-group-item list-group-item-action ">About</a>
            </div>
          </div>
        </div>
        <nav class="navbar navbar-dark">
          <button class="navbar-toggler" @click="menuClick" type="button">
            <span class="icon-bar before"></span>
            <span class="icon-bar main"></span>
            <span class="icon-bar after"></span>
          </button>
        </nav>
      </div>
    </div>
</template>
<style scoped lang="less">
  nav *{
    outline:initial;
    border:none;
  }
  .pos-f-t{
    .navbar-dark{
      z-index: 12;
      position:fixed;
      right:15px;
      top:22px;
      padding:0;
      .navbar-toggler{
        border:none;
        padding:0;
        background:none;
        color:black;
        .icon-bar{
          -webkit-border-radius: 0;
          -moz-border-radius: 0;
          border-radius: 0;
          background-color: #151515;
          -webkit-transition: all ease 0.2s;
          -moz-transition: all ease .2s;
          -o-transition: all ease .2s;
          transition: all ease .2s;
        }
        .before{
          margin-bottom:4px;
        }
        .after{
          margin-top:4px;
        }
        .before, .main, .after{
          display: block;
          width: 22px;
          height: 2px;
        }
      }
    }
    #navbarToggleExternalContent{
      position:fixed;
      right:0;
      top:0;
      z-index: 13;
      height:100%;
      background-color:black;
      -webkit-transition: -webkit-transform 400ms ease;
      -moz-transition: -moz-transform 400ms ease;
      -o-transition: -o-transform 400ms ease;
      transition: transform 400ms ease;
      -webkit-transition-property: -webkit-transform,left,right;
      .p-4{
        min-width:280px;
        .list-group-item{
          background-color:transparent;
          color:#666;
          position:relative;
        }
        .collapse{
          margin-left:15px;
          -webkit-transition: margin-left 400ms ease;
          -moz-transition: margin-left 400ms ease;
          -o-transition: margin-left 400ms ease;
          transition: margin-left 400ms ease;
        }
        .list-group-item:hover{
          color:white;

          #demo{
            li{
              a{
                color:#666;
              }
            }
          }
        }
        .list-group-item:hover::before{
          content: "";
          display: inline-block;
          width:2px;
          height:15px;
          background-color:white;
          position:absolute;
          left:10px;
          top:15px;
        }
      }
      .sb-close{
        img{
          padding:10px 15px;
          -ms-filter: "progid:DXImageTransform.Microsoft.Alpha(Opacity=60)";
          -khtml-opacity: .6;
          -moz-opacity: .6;
          opacity: 0.6;
          -webkit-transition: all ease 0.3s;
          -moz-transition: all ease .3s;
          -o-transition: all ease .3s;
          -ms-transition: all ease .3s;
          transition: all ease .3s;
        }
        img:hover{
          opacity: 1;
        }
      }
    }
  }
</style>
<script>
export default {
  name: 'navContent',
  mounted () {
    this.$refs.menuContent.style.opacity = 0
    const menuWidth = this.$refs.menuContent.offsetWidth
    this.$refs.menuContent.style.right = -menuWidth + 'px'
  },
  methods: {
    menuClick () {
      this.$refs.menuContent.style.opacity = 1
      this.$refs.menuContent.style.right = 0
    },
    closeMenu () {
      const menuWidth = this.$refs.menuContent.offsetWidth
      this.$refs.menuContent.style.right = -menuWidth + 'px'
    }
  }
}
</script>
