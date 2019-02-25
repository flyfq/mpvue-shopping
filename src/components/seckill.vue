<template>
  <div class="index-seckill white-bgcolor">
    <div class="seckill-hd">
      <span class="seckill-hd-title  red-color"><i class="fa fa-clock-o" aria-hidden="true"></i> 限时秒杀</span>
      <strong>10点场</strong>
      <div id="time"></div>
      <div class="seckill-hd-r">秒抢好货 <i class="fa fa-angle-right theme-color" aria-hidden="true"></i></div>
    </div>
    <div class="seckill-bd">
      <div class="seckill-wares">
        <div class="swiper-wrapper">
          <div class="swiper-slide seckill-ware" v-for="item of msg" :key="item.productId">
            <navigator :url="'/pages/item/main?id='+item.productId+'?dataName=' + dataName">
              <a href="##">
                <img :src="item.smallImage" alt="">
                <p class="red-color">￥<strong>{{item.vipshopPrice}}</strong></p>
                <del>￥{{item.marketPrice}}</del>
              </a>
            </navigator>
          </div>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
    export default {
      props:["msg","dataName"],
      data(){
        return{

        }
      },
      mounted(){

      }
    }
</script>

<style scoped>
  * {
    margin: 0;
    padding: 0;
  }
  .white-bgcolor {
    background: #fff !important;
  }
  * {
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
  }
  .red-color {
    color: #ff0000;}
    .seckill-hd-title{
      font-size: 16px;}
  b, strong{
    font-weight: 700;
  }
  .fa {
    display: inline-block;
    font: normal normal normal 14px/1 FontAwesome;
    font-size: inherit;
    text-rendering: auto;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
  }

  .index-seckill{}
  .index-seckill .seckill-hd{
    position: relative;
    height: 30px;
    padding: 0 10px;
    margin-bottom: 8px;
  }
  span.seckill-hd-title.theme-color {
    font-weight: bold;
    font-size: 20px;
  }
  .index-seckill .seckill-hd strong{
    line-height: 30px;
    font-size:12.8px;
    display: inline-block;
  }
  .index-seckill .seckill-hd #time {
    position: absolute;
    top: 0;
    left: 42%;
    line-height: 30px;
  }
  .seckill-hd #time span{
    padding: 0 3px;
    border: 1px solid #dedede;
    border-radius: 4px;
    font-size: 12.8px;
  }
  .index-seckill .seckill-hd-r{
    position: absolute;
    right: 10px;
    top: 0;
    line-height: 30px;
    font-size: 12.8px;
  }

  .index-seckill .seckill-bd{
    width: 100%;
    overflow: hidden;
  }

  .swiper-wrapper {
    position: relative;
    width: 100%;
    height: 100%;
    z-index: 1;
    display: flex;
    box-sizing: content-box;
  }
  swiper-slide seckill-ware swiper-slide-next{
    width: 103.571px;
    margin-right: 5px;
  }
  .swiper-slide{
    flex-shrink: 0;
    height: 100%;
    position: relative;
  }
  img {
    vertical-align: middle;
  }
  .index-seckill .seckill-bd .seckill-wares{}
  .index-seckill .seckill-bd .seckill-wares .seckill-ware{
    width: 83px;   /* 自己后来加上去的 */
    text-align: center;
    padding: 12.8px;
  }

  .seckill-ware img{
    width: 100%;
    height: 88px;

  }
  .seckill-ware p{
    margin: 5px 0 0;
    font-size: 12.8px;
    font-weight: bold;
  }
  .seckill-ware p strong{
    display: inline-block;
    font-size: 20px;
  }
  .seckill-ware del{
    font-size: 12.8px;
    color: #999;
  }
</style>
