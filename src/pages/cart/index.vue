<template>
 <div>
   <form method="post" name="cart_form" target="_self" id="cart_form" action="">
     <header class="zyw-header">
       <div class="zyw-container white-color">
         <div class="head-l"><a href="javascript:window.history.back(-1)" target="_self"><img src="/static/img/svg/head-return.png" alt=""></a></div>
         <h1>购物车</h1>
         <div class="head-r"><a href="">编辑</a></div>
       </div>
     </header>
     <footer class="zyw-footer">
       <div class="zyw-container white-bgcolor">
         <div class="settle_box">
           <dl class="all_check select">
             <dt>
               <span id="all_pitch_on"></span>
               <em>全选</em>
             </dt>
           </dl>
           <dl class="total_amount">
             <dt>
               合计：
               <p id="total_price">
                 ¥<b>0</b>
               </p>
             </dt>
             <dd>不含运费</dd>
           </dl>
           <!--<input type="hidden" name="gcs" id="gcs"/>-->
           <a class="settle_btn" href="javascript:void(0);" id="confirm_cart">去结算</a>
           <a class="settle_btn" href="javascript:void(0);" id="confirm_cart1" onclick="big_cart_remove()">删除</a>
         </div>
       </div>
     </footer>
     <section class="zyw-container">
       <!--list-->
       <div class="commodity_list_box">
         <div class="cart_top">
           <span>商品清单</span>
           <p id="weights">总重量约25kg</p>
           <div class="clear"></div>
         </div>
         <!--商品列表-->
         <div class="commodity_box">
           <div class="commodity_list">
             <!--店名信息-->
             <div class="tite_tim select">
               <em aem="1" cart_id="84"></em>
               <span>Apple产品专营店</span>
               <div class="clear"></div>
             </div>
             <!--商品-->
             <ul class="commodity_list_term">
               <li class="select">
                 <em aem="0" cart_id="84"></em>
                 <img src="https://img13.360buyimg.com/mobilecms/s140x140_jfs/t3229/10/2021133198/376218/cfcc06cb/57d8e84eNfe92eae8.jpg"/>
                 <div class="div_center">
                   <h4>新疆苹果</h4>
                   <span>50斤</span>
                   <p class="now_value">
                     <i>￥</i>
                     <b class="qu_su">123.00</b>
                   </p>
                 </div>
                 <div class="div_right">
                   <i onclick="reducew(this)">-</i>
                   <span class="zi">1</span>
                   <input type="hidden" value="84">
                   <i onclick="plusw(this)">+</i>
                 </div>
               </li>
               <li class="select">
                 <em aem="0" cart_id="84"></em>
                 <img src="https://img13.360buyimg.com/mobilecms/s140x140_jfs/t3229/10/2021133198/376218/cfcc06cb/57d8e84eNfe92eae8.jpg"/>
                 <div class="div_center">
                   <h4>新疆苹果</h4>
                   <span>50斤</span>
                   <p class="now_value">
                     <i>￥</i>
                     <b class="qu_su">25.00</b>
                   </p>
                 </div>
                 <div class="div_right">
                   <i onclick="reducew(this)">-</i>
                   <span class="zi">1</span>
                   <input type="hidden" value="84">
                   <i onclick="plusw(this)">+</i>
                 </div>
               </li>
             </ul>
             <!--优惠信息-->
             <div class="shop_ul_bottom account_info_box">
               <ul class="account_info">
                 <li class="i_text">
                   <span class="info_name xi_cu">包邮</span>
                   <span class="info_name">商家包邮</span>
                 </li>
               </ul>
             </div>
           </div>
         </div>
         <div class="commodity_box">
           <div class="commodity_list">
             <!--店名信息-->
             <div class="tite_tim select">
               <em aem="1" cart_id="84"></em>
               <span>Apple产品专营店</span>
               <div class="clear"></div>
             </div>
             <!--商品-->
             <ul class="commodity_list_term">
               <li class="select">
                 <em aem="0" cart_id="84"></em>
                 <img src="https://img13.360buyimg.com/mobilecms/s140x140_jfs/t3229/10/2021133198/376218/cfcc06cb/57d8e84eNfe92eae8.jpg"/>
                 <div class="div_center">
                   <h4>新疆苹果</h4>
                   <span>50斤</span>
                   <p class="now_value">
                     <i>￥</i>
                     <b class="qu_su">210.00</b>
                   </p>
                 </div>
                 <div class="div_right">
                   <i onclick="reducew(this)">-</i>
                   <span class="zi">1</span>
                   <input type="hidden" value="84">
                   <i onclick="plusw(this)">+</i>
                 </div>
               </li>
               <li class="select">
                 <em aem="0" cart_id="84"></em>
                 <img src="https://img13.360buyimg.com/mobilecms/s140x140_jfs/t3229/10/2021133198/376218/cfcc06cb/57d8e84eNfe92eae8.jpg"/>
                 <div class="div_center">
                   <h4>新疆苹果</h4>
                   <span>50斤</span>
                   <p class="now_value">
                     <i>￥</i>
                     <b class="qu_su">412.00</b>
                   </p>
                 </div>
                 <div class="div_right">
                   <i onclick="reducew(this)">-</i>
                   <span class="zi">1</span>
                   <input type="hidden" value="84">
                   <i onclick="plusw(this)">+</i>
                 </div>
               </li>
             </ul>
             <!--优惠信息-->
             <div class="shop_ul_bottom account_info_box">
               <ul class="account_info">
                 <li class="i_text">
                   <span class="info_name xi_cu">包邮</span>
                   <span class="info_name">商家包邮</span>
                 </li>
               </ul>
             </div>
           </div>
         </div>
         <!-- 商品列表 end -->
       </div>
       <!-- end -->
     </section>
   </form>
 </div>
</template>

<script>


export default {
  data () {
    return {

    }
  },

  components: {

  },

  methods: {

  },

  created () {
    // let app = getApp()
  }
}
</script>

<style scoped>
  .zyw-header {
    top: 0;
    height: 45px;
    line-height: 45px;
    background: url(data:image/jpeg;base64,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) no-repeat;
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
  .settle_box {
    background: #fff;
    position: fixed;
    left: 0px;
    bottom: 0px;
    overflow: hidden;
    z-index: 2;
    width: 100%;
    padding: 0 0 0 4%;
    border-top: solid 1px #e6e6e6;

  }
  .settle_box .all_check {
    width: 17%;
    margin-bottom: 0;
    margin-top: 15px;
  }
  .settle_box .all_check, .settle_box .total_amount {
    float: left;
  }
  .settle_box .total_amount {
    color: #999;
    font-size: 14px;
    margin: 0;
    width: 50%;
    text-align: right;
    /*margin-top: 5px;*/
    /*padding-right: 10px;*/
  }
  .settle_box .all_check span {
    width: 20px;
    height: 20px;
    border: solid 1px #a2a2a2;
    vertical-align: middle;
    border-radius: 50%;
    float: left;
  }
  .settle_box .all_check em {
    font-weight: initial;
    font-size: 13px;
    color: #666;
    margin-left: 10%;
    font-style: normal;
  }
  .settle_box .settle_btn {
    float: right;
    width: 33%;
    background: #f34347;
    color: #fff;
    padding: 17px 0;
    text-align: center;
    font-size: 18px;
  }
  a {
    color: inherit;
    text-decoration: none !important;
  }
  #confirm_cart1 {
    display: none;
  }
  .settle_box .total_amount dt {
    font-weight: initial;
  }
  dd, dt {
    line-height: 1.42857143;
  }
  .settle_box .total_amount dd {
    margin-top: 1px;
    clear: both;
    font-size: 14px;
  }
  dd {
    margin-left: 0;
  }
  .settle_box .total_amount dt p {
    color: #f34347;
    font-size: 14px;
    float: right;
    line-height: 20px;
  }
  .zyw-footer p {
    margin: 0;
  }
</style>
