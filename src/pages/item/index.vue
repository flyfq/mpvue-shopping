<template>
 <div>
   <header class="zyw-header">
     <div class="zyw-container white-color">
       <div class="head-l"><a href="javascript:window.history.back(-1)" target="_self"><img src="/static/img/svg/head-return.png" alt=""></a></div>
       <h1><a href="#" class="active">商品</a><a>详情</a><a href="">评价</a></h1>
       <div class="head-r"><img src="/static/img/svg/head-more.png" alt=""></div>
     </div>
   </header>
   <footer class="zyw-footer">
     <div class="zyw-container white-bgcolor clearfix">
       <div class="col-sm-2 col-xs-2">
         <a class="weui-tabbar__item">
           <div class="weui-tabbar__icon">
             <img src="/static/img/svg/item-1.png" alt="">
           </div>
           <p class="weui-tabbar__label">店铺</p>
         </a>
       </div>
       <div class="col-sm-2 col-xs-2">
         <a class="weui-tabbar__item">
           <span class="weui-badge" style="position: absolute;top: -.4em;right: 1em;">8</span>
           <div class="weui-tabbar__icon">
             <img src="/static/img/svg/item-2.png" alt="">
           </div>
           <p class="weui-tabbar__label">购物车</p>
         </a>
       </div>
       <div class="col-sm-2 col-xs-2">
         <a class="weui-tabbar__item">
           <div class="weui-tabbar__icon">
             <img src="/static/img/svg/item-3.png" alt="">
           </div>
           <p class="weui-tabbar__label">收藏</p>
         </a>
       </div>
       <div class="col-sm-3 col-xs-3">
         <a href="" class="footer-btn footer-warning">立即购买</a>
       </div>
       <div class="col-sm-3 col-xs-3">
         <a href="" class="footer-btn footer-danger">加入购物车</a>
       </div>
     </div>
   </footer>
   <section class="zyw-container">
     <!-- Swiper -->
     <div class="item-img">
       <div class="swiper-wrapper">
         <div class="swiper-slide"><img :src="itemlist.smallImage" alt=""></div>
         <div class="swiper-slide"><img :src="itemlist.image3" alt=""></div>
         <div class="swiper-slide"><img :src="itemlist.image3" alt=""></div>
         <div class="swiper-slide"><img :src="itemlist.image3" alt=""></div>
         <div class="swiper-slide"><img :src="itemlist.image3" alt=""></div>
       </div>
       <!-- Add Pagination -->
       <div class="swiper-pagination"></div>
     </div>
     <div class="item-details white-bgcolor clearfix">
       <h3 class="details-title">{{itemlist.productName}}</h3>
       <strong class="details-prince theme-color pull-left">￥{{itemlist.vipshopPrice}}</strong>
       <span class="details-volume pull-right">月销：{{itemlist.newCatId}}件</span>
     </div>
     <div class="item-choose weui-cells mt-625">
       <a class="weui-cell weui-cell_access open-popup" href="javascript:;" data-target="#item_spec">
         <div class="weui-cell__bd">
           <p class="choose-text">选择 <span>颜色分类</span></p>
         </div>
         <div class="weui-cell__ft choose-des">
         </div>
       </a>
       <div id="item_spec" class="weui-popup__container popup-bottom">
         <div class="weui-popup__overlay"></div>
         <div class="weui-popup__modal">
           <div class="item-spec-layer white-bgcolor">
             <div class="spec-head clearfix">
               <div class="spec-head-img"><img src="https://m.360buyimg.com/n1/jfs/t15787/353/109633918/16701/5a8390ef/5a27ae6dNc530b5bb.jpg!q70.jpg" alt=""></div>
               <strong class="spec-head-prince theme-color">￥7800.00</strong>
               <p class="spec-head-intro">商品编号：51867</p>
             </div>
             <div class="spec-info clearfix">
               <div class="spec-info-hd">颜色</div>
               <div class="spec-info-bd">
                 <ul>
                   <li class="active">银色</li>
                   <li>深空灰色</li>
                 </ul>
               </div>
             </div>
             <div class="spec-info clearfix">
               <div class="spec-info-hd">版本</div>
               <div class="spec-info-bd">
                 <ul>
                   <li>64GB</li>
                   <li class="active">256GB</li>
                   <li>64GB+一年碎屏险套餐</li>
                   <li>256GB+一年碎屏险套餐</li>
                 </ul>
               </div>
             </div>
             <div class="spec-length mb-625">
               <div class="weui-cell__bd">
                 <p class="length-hd">数量</p>
               </div>
               <div class="weui-cell__ft">
                 <div class="weui-count">
                   <a class="weui-count__btn weui-count__decrease"></a>
                   <input class="weui-count__number" type="number" value="1">
                   <a class="weui-count__btn weui-count__increase"></a>
                 </div>
               </div>
             </div>
             <button class="item-layer-button theme-bgcolor white-color" type="submit">确定</button>
             <a href="javascript:;" class="close-popup spec-close"><i class="fa fa-close"></i></a>
           </div>
         </div>
       </div>
       <a class="weui-cell weui-cell_access open-popup" href="javascript:;" data-target="#item_parameter">
         <div class="weui-cell__bd">
           <p class="choose-text">产品参数</p>
         </div>
         <div class="weui-cell__ft choose-des">
         </div>
       </a>
       <div id="item_parameter" class="weui-popup__container popup-bottom">
         <div class="weui-popup__overlay"></div>
         <div class="weui-popup__modal">
           <div class="item-parameter-layer white-bgcolor">
             <h3 class="parameter-title">产品参数</h3>
             <table class="table table-condensed parameter-table">
               <tr>
                 <th>品牌</th>
                 <td>Apple/苹果</td>
               </tr>
               <tr>
                 <th>Apple型号</th>
                 <td>Apple X</td>
               </tr>
               <tr>
                 <th>网络类型</th>
                 <td>无需合约版</td>
               </tr>
               <tr>
                 <th>机身颜色</th>
                 <td>深空灰色 银色</td>
               </tr>
               <tr>
                 <th>套餐类型</th>
                 <td>官方标配</td>
               </tr>
               <tr>
                 <th>售后服务</th>
                 <td>全国联保</td>
               </tr>
               <tr>
                 <th>存储容量</th>
                 <td>256GB 64GB</td>
               </tr>
             </table>
             <button class="item-layer-button theme-bgcolor white-color close-popup" type="submit">完成</button>
           </div>
         </div>
       </div>
     </div>
     <div class="item-serve">
       <span><i class="fa fa-check-circle-o theme-color"></i> 品质承诺</span>
       <span><i class="fa fa-check-circle-o theme-color"></i> 七天包退换</span>
       <span><i class="fa fa-check-circle-o theme-color"></i> 如实描述</span>
     </div>
     <div class="item-assess weui-cells mb-625">
       <a class="weui-cell weui-cell_access" href="javascript:;">
         <div class="weui-cell__bd">
           <p class="choose-text">用户评价（<em class="theme-color">0</em>条）</p>
         </div>
         <div class="weui-cell__ft choose-des">
           100%好评
         </div>
       </a>
     </div>
     <div class="item-precent white-bgcolor" id="item-precent">
       <h4>图文详情</h4>
       <span>
	            <img :src="itemlist.smallImage" alt="">
	            <img :src="itemlist.image3" alt="">
	            <img :src="itemlist.image7" alt="">
	            <br>
	        </span>
     </div>
   </section>
 </div>
</template>

<script>


export default {
  data () {
    return {
      id:"",
      itemlist:{}
    }
  },

  components: {

  },

  methods: {

  },

  beforeMount () {
    // console.log(this.$root.$mp)
    // let app = getApp()
    this.id=this.$root.$mp.query.id

  },
  mounted(){
    let that=this
    wx.request({
      url: 'https://www.wakakale.top:443/item', // 仅为示例，并非真实的接口地址
      data: {
       id:that.id
      },
      header: {
        'content-type': 'application/json' // 默认值
      },
      success(res) {
        console.log(res.data[that.id-1])
        that.itemlist=res.data[that.id-1]
      }
    })
  }

}
</script>

<style scoped>
  .zyw-header {
    top: 0;
    height: 45px;
    line-height: 45px;
    background: url(data:image/jpeg;base64,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) no-repeat center;
    background-size: 100%;
  }
  .zyw-header, .zyw-footer {
    position: fixed;
    width: 100%;
    z-index: 5;
    left: 0;
  }
  header,section{
    display: block;
  }
  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }
  .white-color {
    color: #fff !important;
  }
  .zyw-container {
    width: 100%;
    max-width: 640px;
    margin: 0 auto;
    position: relative;
  }
  .zyw-header .head-l {
    position: absolute;
    top: 0;
    font-size: 18px;
    left: 10px;
  }
  .zyw-header h1 {
    text-align: center;
    font-size: 18px;
    margin: 0;
    line-height: 45px;
  }
  h1{
    font-family: inherit;
    font-weight: 500;
    color: inherit;
  }
  .zyw-header .head-r {
    position: absolute;
    top: 0;
    font-size: 18px;
    right: 10px;
  }
  .zyw-header .head-r img {
    vertical-align: middle;
    width: 20px;
    height: 20px;
  }
  a img {
    border: 0;
    vertical-align: middle;
    height: 20px;
    width: 20px;
  }
  .zyw-header h1 a.active {
    font-weight: bold;
    color: #fff;
  }
  .zyw-header h1 a {
    font-size: 18px;
    padding: 0 18px;
    color: #f5f5f5;
    display: inline-block;
  }
  .zyw-footer {
    bottom: 0;
    height: 56px;
  }
  .btn-group-vertical>.btn-group:after, .btn-group-vertical>.btn-group:before, .btn-toolbar:after, .btn-toolbar:before, .clearfix:after, .clearfix:before, .container-fluid:after, .container-fluid:before, .container:after, .container:before, .dl-horizontal dd:after, .dl-horizontal dd:before, .form-horizontal .form-group:after, .form-horizontal .form-group:before, .modal-footer:after, .modal-footer:before, .modal-header:after, .modal-header:before, .nav:after, .nav:before, .navbar-collapse:after, .navbar-collapse:before, .navbar-header:after, .navbar-header:before, .navbar:after, .navbar:before, .pager:after, .pager:before, .panel-body:after, .panel-body:before, .row:after, .row:before {
    display: table;
    content: " ";
  }
  :after, :before {
    -webkit-box-sizing: border-box;
    -moz-box-sizing: border-box;
    box-sizing: border-box;
  }
  .btn-group-vertical>.btn-group:after, .btn-toolbar:after, .clearfix:after, .container-fluid:after, .container:after, .dl-horizontal dd:after, .form-horizontal .form-group:after, .modal-footer:after, .modal-header:after, .nav:after, .navbar-collapse:after, .navbar-header:after, .navbar:after, .pager:after, .panel-body:after, .row:after {
    clear: both;
  }
  .btn-group-vertical>.btn-group:after, .btn-group-vertical>.btn-group:before, .btn-toolbar:after, .btn-toolbar:before, .clearfix:after, .clearfix:before, .container-fluid:after, .container-fluid:before, .container:after, .container:before, .dl-horizontal dd:after, .dl-horizontal dd:before, .form-horizontal .form-group:after, .form-horizontal .form-group:before, .modal-footer:after, .modal-footer:before, .modal-header:after, .modal-header:before, .nav:after, .nav:before, .navbar-collapse:after, .navbar-collapse:before, .navbar-header:after, .navbar-header:before, .navbar:after, .navbar:before, .pager:after, .pager:before, .panel-body:after, .panel-body:before, .row:after, .row:before {
    display: table;
    content: " ";
  }
  :after, :before {
    box-sizing: border-box;
  }
  .zyw-footer .col-sm-2, .zyw-footer .col-sm-3, .zyw-footer .col-xs-2, .zyw-footer .col-xs-3 {
    padding: 0;
    border-top: 1px solid #f6f6f6;
  }
  .col-xs-2 {
    width:63px;
    height: 51px;
    float: left;
    background-color: #ffffff;
  }
  .col-sm-2,.col-xs-2,.col-xs-3, .col-sm-3{
    position: relative;
    min-height: 1px;
  }
  .col-xs-3 {
    width: 94px;
    float: left
  }
  .toolbar, .weui-tabbar__item {
    position: relative;
  }
  .weui-tabbar__item {
    display: block;
    flex: 1;
    padding: 5px 0 0;
    font-size: 0;
    color: #999;
    text-align: center;
    -webkit-tap-highlight-color: rgba(0,0,0,0);
  }
  .weui-tabbar__icon {
    display: inline-block;
    width: 27px;
    height: 27px;
  }
  .zyw-footer p {
    margin: 0;
  }
  .weui-tabbar__label {
    text-align: center;
    color: #999;
    font-size: 10px;
    line-height: 1.8;
  }
  .weui-tabbar__icon img {
    width: 27px;
    height: 27px;
  }
  .zyw-footer .footer-warning {
    background: orange;
  }
  .zyw-footer .footer-btn {
    line-height: 56px;
    display: inline-block;
    width: 100%;
    text-align: center;
    color: #fff;
    font-size: 16px;
  }
  .zyw-footer .footer-danger {
    background: red;
  }
  .zyw-footer .footer-btn {
    line-height: 56px;
    display: inline-block;
    width: 100%;
    text-align: center;
    color: #fff;
    font-size: 16px;
  }
  .zyw-header~.zyw-container {
    border-top: 45px solid transparent;
  }
  .zyw-footer~.zyw-container {
    border-bottom: 56px solid transparent;
  }
  .item-img {
    width: 100%;
    overflow: hidden;
    position: relative;
  }
  .item-details {
    padding: 16px 10px;
  }
  .white-bgcolor {
    background: #fff !important;
  }
  .mt-625 {
    margin-top: 10px;
    margin-bottom: 0;
  }
  .weui-cells {

    background-color: #fff;
    line-height: 1.47058824;
    font-size: 17px;
    overflow: hidden;
    position: relative;
  }
  .item-serve {
    line-height: 48px;
    padding: 0 10px;
  }
  .mb-625 {
    margin-bottom:10px;
    margin-top: 0;
  }
  .item-precent {
    padding: 5px 0;
  }
  .item-details .details-title {
    font-size: 20px;
    font-weight: bold;
    line-height: 32px;
    overflow: hidden;
    text-overflow: ellipsis;
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-line-clamp: 2;
  }
  .h1, .h2, .h3, .h4, .h5, .h6, h1, h2, h3, h4, h5, h6 {
    font-family: inherit;
    color: inherit;
  }
  .item-details .details-prince {
    font-size: 24px;
  }
  .theme-color {
    color: #956bff !important;
  }
  .pull-left {
    float: left!important;
  }
  b, strong {
    font-weight: 700;
  }
  .item-details .details-volume {
    font-size: 20px;
    color: #999;
  }

  .item-details .details-volume {
    font-size: 20px;
    color: #999;
  }
  .item-details .details-volume {
    font-size: 10px;
    color: #999;
  }
  .weui-cells .weui-cell {
    border-bottom: 1px solid #f6f6f6;
  }
  .weui-cell_access {
    -webkit-tap-highlight-color: rgba(0,0,0,0);
    color: inherit;
  }
  .weui-popup__container {
    display: none;
  }
  .weui-popup__container, .weui-popup__overlay {
    position: fixed;
    bottom: 0;
    left: 0;
    right: 0;
    width: 100%;
    height: 100%;
    z-index: 10;
  }
  .weui-cell_access .weui-cell__ft {
    /* padding-right: 13px; */
    position: relative;
  }
  .choose-text {
    margin: 0;
    font-size: 20px;
    color: #999;
    height:40px;
    line-height: 40px;
  }
  .choose-text span {
    margin-left: 2rem;
    max-width: 50%;
    color: #444;
    overflow: hidden;
    text-overflow: ellipsis;
    word-break: keep-all;
    white-space: nowrap;
  }
  .weui-cell_access .weui-cell__ft {
    /* padding-right: 13px; */
    position: relative;
  }
  .choose-des {
    font-size: 1rem;
  }
  .weui-cell__ft {
    text-align: right;
    color: #999;
  }
</style>
