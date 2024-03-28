<template>

  <view class="content">
    <view class="items">

      <view class="mode">

        <view class="item1">
          <view>
            <image
                src="@/static/lws.jpg"
                mode="scaleToFill"
            />
          </view>

        </view>
        <view class="item2" @click="navigateToGuahao">
          <view class="text1">代挂号预约</view>
          <view class="text2">代挂号预约</view>
          <view class="text3">$10/次</view>
        </view>
      </view>
      <view class="mode">

        <view class="item1">
          <view>
            <image
                src="@/static/lws.jpg"
                mode="scaleToFill"
            />
          </view>
        </view>
        <view class="item2">
          <view class="text1">代问诊预约</view>
          <view class="text2">代问诊预约</view>
          <view class="text3">$10/次</view>
        </view>
      </view>
      <view class="mode">

        <view class="item1">
          <view>
            <image
                src="@/static/lws.jpg"
                mode="scaleToFill"
            />
          </view>
        </view>
        <view class="item2" @click="navigateToQuyao">
          <view class="text1">代取药预约</view>
          <view class="text2">代取药预约</view>
          <view class="text3">$10/次</view>
        </view>
      </view>
    </view>
    </view>
  </template>
  
  <script>
  export default {
    data() {
      return {
        //
      };
    },
    methods: {
      navigateToGuahao() {
        uni.navigateTo({
          url: '/pages/booking/guahao/guahao' // 挂号
        })
      },
      navigateToQuyao() {
        uni.navigateTo({
          url: '/pages/quyao/quyao' // 挂号
        })
      },
  }
}
  </script>
  
  <style>
  .content{
    background-color: #F1F6FC;
    height: 100vmax;
  }
  
  .mode{
    display: flex;
    /* flex-direction: column;
    align-items: center; */
    justify-content: space-between; /* 两个项目之间的距离最大化 */
    background-color: rgb(255, 255, 255);
    height: 100px;
    margin: 20px;
    align-items: center;
    border-radius: 10px;
    
  }
  .mode .item1{
    width: 20%; 
  }
  .mode .item2{
    width: 70%; 
    
  }
  .mode .item1 view{
    padding: 10px;
    

    
  }
  .mode .item1 view image{
    width: 80px; 
    height: 80px;
    border-radius: 10px;
    
    
  }
  .text1{
    font-size: 18px;
  }
  .text2{
    font-size: 12px;
    margin-right: 10px;
  }
  .text3{
    font-size: 20px;
    color: #d80000;
  }
  
  </style>
  