<template>
  <header class="main-header">
      <div class="header-content">
          <h2>
              <img :src="logoUrl">花间博客
          </h2>
          <div class="right-menu">
              <div class="menu-wrapper">
                  <div class="menu-item">
                      <a href="#">首页</a>
                  </div>
                  <div class="menu-item"><a href="#">我的消息</a></div>
                  <div class="menu-item"><a href="#">通知</a></div>
                  <div class="menu-item item-split"><a href="#">登录</a></div>
              </div>
          </div>
      </div>
  </header>
</template>

<script>
export default {
    name:'MainHeader',
    data(){
        return {
            logoUrl:""
        }
    },
    created(){
        let url="assets/logo_huajian.png";
        this.logoUrl=require("@/"+url);
    }
}
</script>

<style scoped>
    .main-header{
        position: fixed;
        z-index: 10;
        top:0;
        margin: 0;
        width: 100%;
        height: 60px;
        /* border-bottom: 1px solid #d64a74; */
        box-shadow: 0 0 10px #d64a74;
        background:rgb(255 255 255 / 14%);
    }
    .header-content{
        display: flex;
        height: 100%;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
        padding:0 100px;
        margin:0 auto;
        font-weight: 400;
        font-size: 14px;
        line-height: 60px;
    }
    .header-content h2 img{
        height: 32px;
        vertical-align: middle;
    }
    .right-menu{
        color:#d64a74;
    }
    .menu-wrapper{
        display: flex;
        justify-content:center;
        align-items: center;
    }
    .menu-wrapper>.menu-item{
        padding:0 20px;
    }
    .menu-wrapper>.menu-item a{
        color:#8f8d8d;
        text-decoration: none;
    }
    .menu-wrapper>.menu-item a:hover{
        color:#d64a74;
    }
    .menu-wrapper>.item-split.menu-item{
        position: relative;
        margin-left:64px;
    }
    .menu-wrapper>.item-split.menu-item:before{
        content:"";
        display: block;
        height: 10px;
        position: absolute;
        bottom: 27px;
        left: -32px;
        border-right: 1px solid #bbbfc4;
        box-sizing: border-box;
    }
</style>