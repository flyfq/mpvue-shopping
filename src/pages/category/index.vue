<template>
  <div>
  <!--<header class="zyw-header">-->
    <!--<div class="zyw-container white-color">-->
      <!--<div class="head-l"><a href="javascript:window.history.back(-1)" target="_self"><img src="/static/img/svg/head-return.png" alt=""></a></div>-->
      <!--<div class="head-search">-->
        <!--<i class="fa fa-search" aria-hidden="true"></i>-->
        <!--<input type="text" placeholder="输入您当前要搜索的商品" class="white-color">-->
      <!--</div>-->
      <!--<div class="head-r"><a href="">取消</a></div>-->
    <!--</div>-->
  <!--</header>-->
  <section class="zyw-container">
    <div class="class-cont clearfix">
      <ul id="myTab" class="nav nav-tabs nav-stacked class-hd">
        <li v-for="item in tabs" :key="index" @click="check(item)"><a data-toggle="tab">{{item}}</a></li>
      </ul>
      <div id="myTabContent" class="tab-content class-bd white-bgcolor">
        <div :class='["tab-pane fade in",show1==true ? "active" : ""]' id="nznz">
          <div class="class-bd-cont">
            <div class="bd-box">
              <h4 class="bd-box-title">热卖选购</h4>
              <div class="bd-box-info">
                <div class="row">
                  <div class="col-xs-4 info-item">
                    <img src="https://img13.360buyimg.com/focus/jfs/t13111/296/562407882/5437/708e24a6/5a0ebc62Nec865e68.jpg" alt="">
                    <p>时尚羽绒</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img30.360buyimg.com/focus/jfs/t13912/250/565576531/4969/64afff47/5a0ebc5cNe2bddf32.jpg" alt="">
                    <p>保暖棉服</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img11.360buyimg.com/focus/jfs/t12559/159/597184401/2349/d2e74b56/5a0ebc54N07bbacf3.jpg" alt="">
                    <p>修身夹克</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img20.360buyimg.com/focus/jfs/t11629/115/2055948200/3740/55436dda/5a0ebc4eN9436e96b.jpg" alt="">
                    <p>牛仔裤</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img11.360buyimg.com/focus/jfs/t13936/183/588130813/8839/9813c67b/5a0e7d9dNbe49c231.jpg" alt="">
                    <p>加厚牛仔</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img10.360buyimg.com/focus/jfs/t12772/63/745865953/4030/e85071ec/5a12b220N009d72a4.jpg" alt="">
                    <p>宽松卫衣</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img12.360buyimg.com/focus/jfs/t12346/326/736792997/3041/8c591fbc/5a1284e4N5f6ac63d.jpg" alt="">
                    <p>连衣裙</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img11.360buyimg.com/focus/jfs/t11296/167/2160342769/2309/f04ca6ca/5a126a5aN99085a6b.jpg" alt="">
                    <p>婚纱</p>
                  </div>
                </div>
              </div>
            </div>
            <div class="bd-box">
              <h4 class="bd-box-title">女装</h4>
              <div class="bd-box-info">
                <div class="row">
                  <div class="col-xs-4 info-item">
                    <img src="https://img10.360buyimg.com/focus/jfs/t13465/116/726666318/2650/623a7359/5a12b23eNbc0d7a47.jpg" alt="">
                    <p>新款大衣</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img20.360buyimg.com/focus/jfs/t14179/99/752605750/2297/f82b2e3d/5a12b234N2259963f.jpg" alt="">
                    <p>连衣裙</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img30.360buyimg.com/focus/jfs/t11794/114/2228059199/2529/60e8b474/5a12b21eN10fd877c.jpg" alt="">
                    <p>针织衫</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img30.360buyimg.com/focus/jfs/t13516/94/713391824/4978/97513273/5a12b228Nf46f2ff1.jpg" alt="">
                    <p>毛衣</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img10.360buyimg.com/focus/jfs/t12772/63/745865953/4030/e85071ec/5a12b220N009d72a4.jpg" alt="">
                    <p>宽松卫衣</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img13.360buyimg.com/focus/jfs/t13774/60/747129929/2709/b436419d/5a12b217N8470eba0.jpg" alt="">
                    <p>外套</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img12.360buyimg.com/focus/jfs/t12409/127/746361250/2852/a7e2c78f/5a12b214Na8e5f494.jpg" alt="">
                    <p>阔腿裤</p>
                  </div>
                </div>
              </div>
            </div>
            <div class="bd-box">
              <h4 class="bd-box-title">童装</h4>
              <div class="bd-box-info">
                <div class="row">
                  <div class="col-xs-4 info-item">
                    <img src="https://img12.360buyimg.com/focus/jfs/t11257/255/2211172737/8332/3ef32977/5a12448aN04e0b987.jpg" alt="">
                    <p>品质童装</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img12.360buyimg.com/focus/jfs/t12442/247/704086578/7163/f0b3677d/5a12447fNd3894b27.jpg" alt="">
                    <p>套装</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img10.360buyimg.com/focus/jfs/t13756/13/712950885/7910/6346b45/5a124475Nb3b9efd6.jpg" alt="">
                    <p>裙子</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img12.360buyimg.com/focus/jfs/t11635/258/2210764394/12510/66bd58cf/5a12445bN917f40bb.jpg" alt="">
                    <p>亲子装</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div :class='["tab-pane fade in",show2==true ? "active" : ""]' class="tab-pane fade" id="nxnx">
          <div class="class-bd-cont">
            <div class="bd-box">
              <h4 class="bd-box-title">流行男鞋</h4>
              <div class="bd-box-info">
                <div class="row">
                  <div class="col-xs-4 info-item">
                    <img src="https://img14.360buyimg.com/focus/jfs/t13807/314/786063079/2610/c0e7de7b/5a139490Nc7fa0e4a.jpg" alt="">
                    <p>休闲鞋</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img30.360buyimg.com/focus/jfs/t13138/355/835254734/2223/adb0cd95/5a139489N23c871c6.jpg" alt="">
                    <p>商务鞋</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img20.360buyimg.com/focus/jfs/t13552/146/765573445/2431/4311417d/5a13947dN5d024b9f.jpg" alt="">
                    <p>正装鞋</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img30.360buyimg.com/focus/jfs/t11992/144/2244194535/2627/3de251a9/5a139564Naee94e4a.jpg" alt="">
                    <p>帆布鞋</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img20.360buyimg.com/focus/jfs/t11608/19/2161730920/5152/2fca75c0/5a13945cN82a4c505.jpg" alt="">
                    <p>板鞋</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img11.360buyimg.com/focus/jfs/t13036/184/750618513/5315/27749ec8/5a13945aN0c00392c.jpg" alt="">
                    <p>乐福鞋</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img20.360buyimg.com/focus/jfs/t13234/118/798001202/2581/6e6cc64d/5a139429N8c5c158d.jpg" alt="">
                    <p>拖鞋</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img14.360buyimg.com/focus/jfs/t11803/345/2212661587/2218/85b38b81/5a139422N611a859c.jpg" alt="">
                    <p>传统布鞋</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img10.360buyimg.com/focus/jfs/t11824/310/2093755858/3582/469cedf4/5a139411N2cd65a08.jpg" alt="">
                    <p>凉鞋</p>
                  </div>
                </div>
              </div>
            </div>
            <div class="bd-box">
              <h4 class="bd-box-title">时尚女鞋</h4>
              <div class="bd-box-info">
                <div class="row">
                  <div class="col-xs-4 info-item">
                    <img src="https://img12.360buyimg.com/focus/jfs/t11215/28/2255245076/2123/34893220/5a13f4c2N878e06ff.jpg" alt="">
                    <p>休闲鞋</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img11.360buyimg.com/focus/jfs/t12391/56/793656945/6443/8dd29335/5a13f4bbN0109307e.jpg" alt="">
                    <p>女靴</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img12.360buyimg.com/focus/jfs/t14071/40/787831338/2452/708b727c/5a13f4b4Ndd40587a.jpg" alt="">
                    <p>短靴</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img30.360buyimg.com/focus/jfs/t12115/73/819992685/2931/f6dd612a/5a13f4adN0116fe8b.jpg" alt="">
                    <p>马丁靴</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img14.360buyimg.com/focus/jfs/t13090/47/771516189/4149/4e90042d/5a13f4a2Ndab62821.jpg" alt="">
                    <p>帆布鞋</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img20.360buyimg.com/focus/jfs/t11425/144/2240698284/6302/25994392/5a13f483Nf8bfdc2a.jpg" alt="">
                    <p>高跟鞋</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img12.360buyimg.com/focus/jfs/t14173/278/783151079/2583/827febf/5a13f446N1df58a24.jpg" alt="">
                    <p>通勤OL</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img30.360buyimg.com/focus/jfs/t12202/143/797781605/8338/ffe87737/5a13f437N94b74f9e.jpg" alt="">
                    <p>凉鞋</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div :class='["tab-pane fade in",show3==true ? "active" : ""]' class="tab-pane fade" id="nyps">
          <div class="class-bd-cont">
            <div class="bd-box">
              <h4 class="bd-box-title">保暖内衣</h4>
              <div class="bd-box-info">
                <div class="row">
                  <div class="col-xs-4 info-item">
                    <img src="https://img30.360buyimg.com/focus/jfs/t11665/278/2197383506/8742/b3a23c67/5a151d25N2927b937.jpg" alt="">
                    <p>保暖内衣</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img10.360buyimg.com/focus/jfs/t14194/47/842495430/4074/ecf95595/5a151c9fNcbf87576.jpg" alt="">
                    <p>保暖裤</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img10.360buyimg.com/focus/jfs/t13972/34/849982121/5216/58243ee9/5a151c97Nf6982faf.jpg" alt="">
                    <p>男士保暖</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img30.360buyimg.com/focus/jfs/t12475/176/848778869/6374/6375ca3d/5a151c91N7eb33b8a.jpg" alt="">
                    <p>女士保暖</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img13.360buyimg.com/focus/jfs/t11809/296/2163842896/4546/352b9a6e/5a151c8bN96fecb7e.jpg" alt="">
                    <p>保暖套装</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img20.360buyimg.com/focus/jfs/t7399/70/3104753877/8744/76f4c985/5a151c86Na4d59a6e.jpg" alt="">
                    <p>秋衣秋裤</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img11.360buyimg.com/focus/jfs/t13735/32/849000445/5947/960b5ef2/5a151c7fNbc7f4c1e.jpg" alt="">
                    <p>薄款保暖</p>
                  </div>
                </div>
              </div>
            </div>
            <div class="bd-box">
              <h4 class="bd-box-title">大牌文胸</h4>
              <div class="bd-box-info">
                <div class="row">
                  <div class="col-xs-4 info-item">
                    <img src="https://img14.360buyimg.com/focus/jfs/t13378/250/854666186/6239/1bf559e7/5a151a72N53143ccc.jpg" alt="">
                    <p>文胸</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img10.360buyimg.com/focus/jfs/t12130/124/832696896/5911/f4d2344a/5a151a6cNdc177f6d.jpg" alt="">
                    <p>文胸套装</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img10.360buyimg.com/focus/jfs/t11482/131/2311710162/3140/d8fde417/5a151a65N45b485d1.jpg" alt="">
                    <p>光面文胸</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img14.360buyimg.com/focus/jfs/t13594/205/852318080/7617/582aed75/5a151a5fN25aee58e.jpg" alt="">
                    <p>少女文胸</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img11.360buyimg.com/focus/jfs/t13153/305/851394568/6118/1820a06f/5a151a59Nbdabaca6.jpg" alt="">
                    <p>大码文胸</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img10.360buyimg.com/focus/jfs/t11308/327/2313435108/3168/9d291152/5a151a53Nae33f47f.jpg" alt="">
                    <p>薄杯文胸</p>
                  </div>
                </div>
              </div>
            </div>
            <div class="bd-box">
              <h4 class="bd-box-title">睡衣</h4>
              <div class="bd-box-info">
                <div class="row">
                  <div class="col-xs-4 info-item">
                    <img src="https://img10.360buyimg.com/focus/jfs/t11005/3/2304642911/8385/a71450ca/5a151858N4be1dc0d.jpg" alt="">
                    <p>女式睡衣</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img13.360buyimg.com/focus/jfs/t12541/211/823596303/8968/f7a77219/5a151865N76835f4e.jpg" alt="">
                    <p>男式睡衣</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img12.360buyimg.com/focus/jfs/t11329/12/1836956333/9157/98620256/5a151865N6a6fad17.jpg" alt="">
                    <p>情侣睡衣</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img30.360buyimg.com/focus/jfs/t13192/199/867844884/7586/76e77fe9/5a151856N09b4ab99.jpg" alt="">
                    <p>全棉睡衣</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img13.360buyimg.com/focus/jfs/t11587/21/2313014983/9146/861f5dae/5a151829Nfecff630.jpg" alt="">
                    <p>珊瑚绒睡衣</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img10.360buyimg.com/focus/jfs/t11851/285/2297627074/5910/155cdfa4/5a1517c4N4ac20e25.jpg" alt="">
                    <p>睡裙</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img20.360buyimg.com/focus/jfs/t12130/215/855565191/6525/9839c527/5a1517c9N65f06d53.jpg" alt="">
                    <p>睡袍</p>
                  </div>
                  <div class="col-xs-4 info-item">
                    <img src="https://img14.360buyimg.com/focus/jfs/t11551/3/2267920652/11096/40692555/5a151679Ne7ced42c.png" alt="">
                    <p>真丝睡衣</p>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  </div>
</template>

<script>


export default {
  data () {
    return {
      show1:true,
      show2:false,
      show3:false,
      tabs:[
        "男装女装","男鞋女鞋","内衣配饰","箱包手袋",
        "美妆个护","钟表珠宝","手机数码","电脑办公",
        "家用电器","食品生鲜","酒水饮料","医药保健",
        "运动户外","家居厨具","汽车用品","图书音像"],
      contents:{
        // yi:[{title:["热卖选购","女装","童装"]},{child1:[],child2:[],child3:[]}],
        // xie:[{title:["流行男鞋","流行女装"]},{child1:[],child2:[],child3:[]}],
        // nei:[{title:["保暖内衣","大牌文胸","睡衣"]},{
        //   child1:["保暖内衣","保暖裤","男士保暖","女士保暖","保暖套装","秋衣保暖","薄款保暖",],
        //   child2:["文胸","文胸套装","光面文胸","少女文胸","大码文胸","薄杯文胸"],
        //   child3:[]}],
      }
    }

  },

  components: {

  },

  methods: {
      check(item){
        // console.log(item)
        if(item=="男装女装"){
          this.show1=true
          this.show2=false
          this.show3=false
        }else if(item=="男鞋女鞋"){
          this.show2=true
          this.show1=false
          this.show3=false
        }else if(item=="内衣配饰"){
          this.show3=true
          this.show2=false
          this.show1=false
        }

      }
  },

  created () {
    // let app = getApp()
  }
}
</script>

<style scoped>
  * {
    box-sizing: border-box;
  }
  .zyw-header {
    top: 0;
    height: 45px;
    line-height: 45px;
    background: url(data:image/jpeg;base64,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) no-repeat;
    background-size: 100%;
    position: fixed;
    width: 100%;
    z-index: 5;
    left: 0;
  }
  header{
    display: block;
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
    top: -7px;
    font-size: 24px;
    left: 10px;
  }
  .zyw-header .head-l a img{
    width: 20px;
    height: 20px;
  }
  .head-search {
    position: relative;
    width: 240px;
    margin-left:45px;
    line-height: 45px;
    margin-top: 8px;
  }
  .head-search input {
    background: #8254bf;
    background: rgba(0, 0, 0, 0.25);
  }
  .head-search input {
    width: 100%;
    height: 30px;
    line-height: 30px;
    border: none;
    padding-left: 30px;
    border-radius: 4px;
    font-size:12px;
  }

  .zyw-header .head-r {
    position: absolute;
    top: -8px;
    font-size: 24px;
    right: 10px;
  }
  .zyw-header .head-r a {
    font-size: 19.2px;
  }
  .zyw-header~.zyw-container {
    border-top: 45px solid transparent;
  }
  .class-cont {
    position: fixed;
    overflow-x: hidden;
    overflow-y: auto;
    height: calc(100% - 101px);
    max-width: 640px;
  }
  .class-cont .class-hd {
    float: left;
    width: 28%;
    height: 100%;
    position: fixed;
    overflow-y: auto;
  }
  .nav-tabs {
    border-bottom: 1px solid #ddd;
  }
  .nav {
    padding-left: 0;
    margin-bottom: 0;
    list-style: none;

  }
  .class-cont .class-hd>li {
    width: 105px;
    border-bottom: 1px solid #e6e6e6;
    text-align: center;
    font-size: 12px;
  }
  .nav-stacked>li+li {
    margin-top: 2px;
    margin-left: 0;
  }
  .nav-stacked>li {
    float: none;
  }
  .nav-tabs>li {
    float: left;
    margin-bottom: -1px;
  }
  .nav>li {
    position: relative;
    display: block;
  }
  li.active{
    background: #f2f2f2;}
  .class-cont .class-hd>li>a {
    line-height: 38.4px;
    margin-right: 0;
  }
  .nav-tabs>li>a {
    margin-right: 2px;
    line-height: 1.42857143;
    border: 1px solid transparent;
    border-radius: 4px 4px 0 0;
  }
  .nav>li>a {
    position: relative;
    display: block;
    padding: 10px 15px;
  }
  /*a {*/
    /*color: #337ab7;*/
    /*text-decoration: none;*/
  /*}*/
  .class-cont .class-hd>li {
    border-bottom: 1px solid #e6e6e6;
    text-align: center;
    font-size: 12px;
  }
  ::-webkit-scrollbar {
    width: 0px;
    background-color: #F5F5F5;
  }
  .class-cont .class-bd {
    float: right;
    width:276px;
    margin-left: 100px;
  }
  .tab-content>.tab-pane {
    display: none;
  }
  .tab-content>.active {
    display: block;
  }
  .fade.in {
    opacity: 1;
  }
  .class-bd-cont {
    padding: 0 16px;
  }
  .class-bd-cont .bd-box .bd-box-title {
    font-size: 14px;
    line-height: 36px;
    color: #777;
  }
  .h4, .h5, .h6, h4, h5, h6 {
    margin-top: 10px;
    margin-bottom: 10px;
  }
  .h1, .h2, .h3, .h4, .h5, .h6, h1, h2, h3, h4, h5, h6 {
    font-family: inherit;
    font-weight: 500;
    line-height: 1.1;
    color: inherit;
  }
  .row {
    width: 276px;
    height: 304px;
    margin-right: -15px;
    margin-left: -15px;
  }
  .class-bd-cont .bd-box .bd-box-info .info-item {
    text-align: center;
    margin-bottom: 16px;
  }
  .col-xs-4 {
    width: 55px;
    float: left;
    position: relative;
    min-height: 1px;
    padding-right: 15px;
    padding-left: 15px;
  }
  .class-bd-cont .bd-box .bd-box-info .info-item img {
    width: 49px;
    height: 49px;
    vertical-align: middle;
    border: 0;
  }
  .class-bd-cont .bd-box .bd-box-info .info-item p {
    font-size: 10px;
    line-height: 30px;
    color: #777;
  }
  p {
    margin: 0 0 10px;
  }
</style>
