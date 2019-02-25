<template>
 <div class="container">
   <swiper  class="my-swipe"
     :indicator-dots="true"
     :autoplay="true"
     :interval="1000"
     :duration="100"
   >
       <swiper-item class="slide1">
         <image class="nav-img" src="https://img.alicdn.com/imgextra/i4/2590951958/TB2Fz6XfgMPMeJjy1XbXXcwxVXa_!!2590951958.jpg" mode="aspectFill" />
       </swiper-item>
     <swiper-item class="slide2">
       <image  class="nav-img" src="https://img.alicdn.com/imgextra/i4/2590951958/TB2z.NKbaagSKJjy0FgXXcRqFXa_!!2590951958.jpg" mode="aspectFill" />
     </swiper-item>
     <swiper-item class="slide3">
       <image class="nav-img" src="https://img.alicdn.com/imgextra/i4/2590951958/TB2ZxVCbjihSKJjy0FeXXbJtpXa_!!2590951958.jpg" mode="aspectFill"/>
     </swiper-item>
   </swiper>
   <navmeau></navmeau>
   <news></news>

     <seckill :msg="msg" dataName="products"></seckill>


   <show></show>
   <wares :msg="msg" dataName="products"></wares>

 </div>
</template>

<script>

import navmeau from "../../components/navmeau";
import news from "../../components/news";
import seckill from "../../components/seckill"
import show from "../../components/show"
import wares from "../../components/wares"
export default {
  data () {
    return {
    msg:[]
    }
  },

  components: {
   navmeau,news,seckill,show,wares
  },

  methods: {

  },
  created () {
    // let app = getApp()
    let that =this
    mpvue.request({
      url: 'https://www.wakakale.top:443/list', // 仅为示例，并非真实的接口地址
      header: {
        'content-type': 'application/json' // 默认值
      },
      success(res) {
        // console.log(res.data)
        that.msg = res.data
        // console.log(that.msg)
      }
    })
  }
}
</script>

<style scoped>
  .container{
    display: flex;
    flex: 1;
    flex-direction: column;
    box-sizing: border-box;
  }
  .my-swipe {
    height: 360rpx;
  }
  .my-swipe .nav-img{width: 100%;
    height: 360rpx;
    vertical-align:middle}

  /*.slide1 {*/
    /*!* background-color: #0089dc; *!*/
    /*color: #fff;*/
  /*}*/

  /*.slide2 {*/
    /*!* background-color: #ffd705; *!*/
    /*color: #000;*/
  /*}*/

  /*.slide3 {*/
    /*!* background-color: #ff2d4b; *!*/
    /*color: #fff;*/
  /*}*/

</style>
