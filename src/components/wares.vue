<template>
  <div class="index-wares">
    <div class="wares-title"><img src="http://gw.alicdn.com/tfs/TB1Aw9JSVXXXXXQXXXXXXXXXXXX-1500-68.png" alt=""></div>
    <div class="wares-cont">
      <ul class="clearfix">
        <li class="col-sm-6 col-xs-6 ware-box" v-for="item of msg" :key="item.productId">
          <navigator :url="'/pages/item/main?id='+item.productId+'?dataName=' + dataName">
            <a href="##">
              <div class="ware-img">
                <img :src="item.smallImage" alt="">
                <span class="ware-vip">vip专享</span>
              </div>
              <h3 class="ware-title">{{item.productName}}</h3>
              <p class="ware-des">{{item.subTitle}}</p>
              <span class="ware-prince red-color">￥{{item.vipshopPrice}}</span>
            </a>
          </navigator>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
    export default {
        props:["msg","dataName"]
    }
</script>

<style scoped>
  ul, ol, li{list-style-type: none;}
  .index-wares{
    width: 100%;
    margin-top: 200px;
  }
  .index-wares .wares-title {
    line-height: 48px;
    text-align: center;
    font-size: 20.8px;
    margin-top: 10px;
  }
  .index-wares .wares-title img{
    width: 100%;
    height: 17px;
  }
  .index-wares .wares-cont{
    margin: 0;
    padding: 0;
    background: #fff;
  }
  .index-wares .wares-cont .ware-box{
    width: 156px;
    height: 256px;
    float: left;
    padding-bottom: 5px;
    border-bottom: 1px solid #f4f4f4;
  }
  .index-wares .wares-cont .ware-box:nth-child(2n+1){
    border-right: 1px solid #f4f4f4;
  }
  .index-wares .wares-cont .ware-box .ware-img{
    position: relative;
    padding: 20px;
  }
  .index-wares .wares-cont .ware-box .ware-img img{
    width: 115px;
    height: 145.5px;
  }
  .index-wares .wares-cont .ware-box .ware-img .ware-vip{
    position: absolute;
    background: #ff6585;
    color: #fff;
    padding: 1px 7px;
    font-size: 12.8px;
    bottom: 0;
    left: 0;
  }
  .index-wares .wares-cont .ware-box .ware-title{
    font-size: 16px;
    line-height: 25px;
    margin: 0;
    word-break: break-all;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
  }
  .index-wares .wares-cont .ware-box .ware-des{
    margin: 0;
    line-height: 20px;
    font-size:14px;
    color: #bbbbbb;
    word-break: break-all;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
  }
  .index-wares .wares-cont .ware-box .ware-prince{
    font-size: 17.6px;
  }

  *, :after, :before {
    -webkit-box-sizing: border-box;
    box-sizing: border-box;
  }

  ol, ul {
    margin-top: 0;
    margin-bottom: 10px;
  }
  .col-sm-6,.col-xs-6{
    position: relative;
    min-height: 1px;
    padding-right: 15px;
    padding-left: 15px;
  }
  p {
    display: block;
    margin-block-start:12px;
    margin-block-end: 12px;
    margin-inline-start: 0px;
    margin-inline-end: 0px;
  }
</style>
