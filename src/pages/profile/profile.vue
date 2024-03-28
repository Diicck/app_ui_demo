<template>
  <view class="content">
    <view class="mys">

      <view class="item1">
        <view>
          <image
              src="@/static/lws.jpg"
              mode="scaleToFill"
          />
        </view>

      </view>
      <view class="item2">
        <view>李文山</view>
        <view>17325665984</view>

      </view>
    </view>

    <view class="btns">

      <view class="btn">订单明细<span>
  <image
      src="@/static/jiantou.png"
      mode="scaleToFill"

  />
</span>


      </view>
      <view class="line"></view>
      <view class="btn">我的团队<span>
  <image
      src="@/static/jiantou.png"
      mode="scaleToFill"
  />
</span></view>
      <view class="line"></view>
      <view class="btn">联系我们<span>
  <image
      src="@/static/jiantou.png"
      mode="scaleToFill"
  />
</span></view>
      <view class="line"></view>
      <view class="btn">加入我们<span>
  <image
      src="@/static/jiantou.png"
      mode="scaleToFill"
  />
</span></view>
      <view class="line"></view>

    </view>
  </view>
</template>
  
  <script>
  export default {
    data() {
      return {
        //
      };
    }
  };
  </script>
  
  <style>
  
  /* Your profile page CSS */


  .content{
    background-color: #ffffff;
    height: 100vh;
    font-family: "PingFang SC",sans-serif;
  }
  .mys{
    
    display: flex;
    /* flex-direction: column;
    align-items: center; */
    justify-content: space-between; /* 两个项目之间的距离最大化 */
    background-color: rgb(43, 110, 255);
    height: 100px;
    align-items: center;
    margin: 10px;
    border-radius: 10px;
    
  }
  .mys .item1{
    width: 20%; 
    padding-left: 20px;
  }
  .mys .item2{
    width: 80%; 
  }
  .item2 view{
    color: white;
    font-weight: bold;
    font-size: 18px;

  }
  .mys .item1 view{
    width: 55px; 
    height: 55px;
    
  }
  .mys .item1 view image{
    width: 50px; 
    height: 50px;
    border-radius: 25px;
    
  }


  .btns {
    margin-top: 10px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
  .btn {
  width: 100%;
  height: 50px;
  
  background-color: rgb(255, 255, 255);
  display: flex;
  justify-content: left;
  align-items: center;
  margin-bottom: 1px;
  font-size: 20px;
  padding-left: 60px;
  border-radius: 10px;

 
}
  .btn span {
  padding-left: 250px;
  
}
  .btn span image {
  width: 10px;
  height: 18px;
  
}
  .line{
   background-color: #c0c0c0;
    height: 1px;
    width: 85%;
  }
  </style>
  