<template>
  <div class="index-news">
    <div class="news-cont white-bgcolor">
      <strong>最新<em>资讯</em>：</strong>
      <div class="infoBox swiper-container-vertical swiper-container-wp8-vertical">
        <ul class="swiper-wrapper">
          <li class="swiper-slide"><a href="#"><span>酷购商城微信版上线啦！</span></a></li>
          <!--<li class="swiper-slide"><a href="#"><span>酷购商城微信版上线啦2！</span></a></li>-->
          <!--<li class="swiper-slide"><a href="#"><span>马上就要开学了，书包买买买！</span></a></li>-->
        </ul>
      </div>
      <ul>
        <li><a href=""></a></li>
      </ul>
      <a href="" class="news-more">更多</a>
    </div>
  </div>
</template>

<script>
    export default {

    }
</script>

<style scoped>
  * {
    box-sizing: border-box;
  }
  *{margin:0;padding:0}
  .white-bgcolor {
    background: #fff !important;
  }
    b, strong {
    font-weight: 700;
  }
  .index-news .news-cont strong em{background: #956bff;}
  /*.swiper-container-wp8-vertical, .swiper-container-wp8-vertical>.swiper-wrapper {*/
    /*!*-ms-touch-action: pan-x;*!*/
    /*touch-action: pan-x;*/
  /*}*/
  /*.swiper-wrapper{*/
    /*position: relative;*/
    /*width: 100%;*/
    /*height: 100%;*/
    /*z-index: 1;*/
    /*display: flex;*/
    /*box-sizing: content-box;*/
    /*transition-duration:300ms;*/
    /*transform: translate3d(0px, 0px, 0px);*/
  /*}*/
  /*.swiper-slide{*/
    /*flex-shrink: 0;*/
    /*width: 100%;*/
    /*position: relative;*/
    /*transition-property:transform,-webkit-transform;*/
  /*}*/
  /*li {*/
    /*display: list-item;*/
    /*text-align: -webkit-match-parent;*/
  /*}*/
  .swiper-wrapper{box-sizing: content-box;}
  .index-news{
    /*background: #ccc;*/
    /*border-top: 1px solid #cccccc;*/
    /*border-bottom: 1px solid #cccccc;*/
    padding: 6.4px 10px;
  }
  .index-news .news-cont{
    position: relative;
    padding: 0 10px;
    height: 30px;
    line-height: 30px;
    border-radius: 4px;
    /*overflow: hidden;*/
  }
  .index-news .news-cont strong{

    position: absolute;
    top: 0;
    left: 10px;
  }
  .index-news .news-cont strong em{
    display: inline-block;
    font-style: normal;
    font-size: 12.8px;
    color: #fff;
    padding: 1px 2px 0;
    margin-left: 2px;
    border-radius: 10px;
  }
  .index-news .infoBox{
    display: inline-block;
  }
  .index-news .news-cont ul{
    list-style-type: none;
    margin: 0;
  }
  .index-news .news-cont ul li{
    line-height: 30px;
  }
  .index-news .news-cont ul li span{
    padding-left: 72px;
    word-break: break-all;
    white-space: nowrap;
    overflow: hidden;
  }
  .index-news .news-cont ul li span i{
    font-style: normal;
    font-size: 12.8px;
    border: 1px solid #fe7900;
    color: #fe7900;
    border-radius: 2px;
    padding: 0 1px;
    margin-right: 5px;
  }
  .index-news .news-cont .news-more{
    position: absolute;
    top: 0;
    right: 0;
    display: inline-block;
    background: #fff;
    padding: 0 10px;
    border-left: 1px solid #f2f2f2;
  }

</style>
