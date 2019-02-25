<template>
  <div class="index-class white-bgcolor">
    <div class="weui-flex">
      <div class="weui-flex__item">
        <a href="javascript:;">
          <div class="index-class-img">
            <img class="meau-img" src="/static/img/yqyl.png" alt="">
          </div>
          <p class="index-class-text">邀请有礼</p>
        </a>
      </div>
      <div class="weui-flex__item">
        <a href="javascript:;">
          <div class="index-class-img">
            <img class="meau-img" src="/static/img/cjfl.png" alt="">
          </div>
          <p class="index-class-text">春节福利</p>
        </a>
      </div>
      <div class="weui-flex__item">
        <a href="javascript:;">
          <div class="index-class-img">
            <img class="meau-img" src="/static/img/kbsc.png" alt="">
          </div>
          <p class="index-class-text">酷币商城</p>
        </a>
      </div>
      <div class="weui-flex__item">
        <a href="javascript:;">
          <div class="index-class-img">
            <img class="meau-img" src="/static/img/sjtx.png" alt="">
          </div>
          <p class="index-class-text">手机通讯</p>
        </a>
      </div>
      <div class="weui-flex__item">
        <a href="javascript:;">
          <div class="index-class-img">
            <img class="meau-img" src="/static/img/sjpj.png" alt="">
          </div>
          <p class="index-class-text">手机配件</p>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>

  .white-bgcolor{background: #fff !important;}
  * {
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
  }
  *{margin:0;padding:0}
  .weui-flex {
    display: -webkit-box;
    display: -webkit-flex;
    display: flex;}
  :after, :before {
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
  }
  .weui-flex__item {
    -webkit-box-flex: 1;
    -webkit-flex: 1;
    flex: 1;}
  .index-class .weui-flex__item {
    text-align: center;
  }
  a {
    color: inherit;
    text-decoration: none !important;
  }
  a {
    background-color: transparent;
    -webkit-tap-highlight-color: rgba(0,0,0,0);
  }
  .index-class .weui-flex__item {
    text-align: center;
  }
  a img {
    border: 0;
  }
  img {
    vertical-align: middle;
    width: 48px;
    height: 48px;
  }
  p {
    display: block;
    margin-block-start: 16px;
    margin-block-end: 16px;
    margin-inline-start: 0px;
    margin-inline-end: 0px;
  }
  .index-class .index-class-text {
    margin: 0;
    line-height: 40px;
    color: #444;
  }
  .index-class{
    padding: 12px 10px;
  }
  .index-class .weui-flex__item{
    text-align: center;
  }
  .index-class .index-class-img{}
  .index-class .index-class-text{
    margin: 0;
    line-height: 40px;
    color: #444;
  }
</style>
