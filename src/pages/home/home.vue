<template>
    <view class="content">
      <view class="imgs">
			<swiper class="swiper" autoplay easing-function="linear">
				<swiper-item>
					<view class="swiper-item">
            <image
              src="@/static/img4.png"
              mode="heightFix"
            />

          </view>
				</swiper-item>
				<swiper-item>
					<view class="swiper-item">
            <image
              src="@/static/img4.png"
              mode="heightFix"
            />
          </view>
				</swiper-item>
				<swiper-item>
					<view class="swiper-item">
            <image
              src="@/static/img4.png"
              mode="heightFix"
            />
          </view>
				</swiper-item>
			</swiper>
		</view>
      <!-- <view class="imgs">
      <swiper

        autoplay
        circular
      >
        <swiper-item>
          <image src="@/static/img2.jpg" mode="scaleToFill"/>
        </swiper-item>
        <swiper-item>
          <image src="@/static/img3.jpg" mode="scaleToFill"/>
        </swiper-item> 
        <swiper-item>
          <image src="@/static/img3.png" mode="scaleToFill"/>
        </swiper-item>
      </swiper>
      </view> --> 
      <view class="btns">

        <view class="btn" @click="navigateToBooking()">
          
          <p>预约服务</p>
          
          <span>
          <image
          src="@/static/jiantou.png"
          mode="scaleToFill"
        />
      </span></view>
        <view class="btn" @click="showDialog()">转诊服务<span>
          <image
          src="@/static/jiantou.png"
          mode="scaleToFill"
        />
        </span></view>
        <view class="btn">住院护理<span>
          <image
          src="@/static/jiantou.png"
          mode="scaleToFill"
        />
        </span></view>
        <view class="btn">养老服务<span>
          <image
          src="@/static/jiantou.png"
          mode="scaleToFill"
        />
        </span></view>

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
      navigateToBooking() {
      uni.navigateTo({
        url: '/pages/booking/booking' // 预约服务
      })
    },
    showDialog() {
      uni.showModal({
        title: '转诊服务', // 对话框标题
        content: '您确定要进行转诊服务吗？', // 对话框内容
        success: function (res) {
          if (res.confirm) {
            console.log('用户点击确定');
            // 用户点击确定后的操作
          } else if (res.cancel) {
            console.log('用户点击取消');
            // 用户点击取消后的操作
          }
        }
      });
    }
  }
}
  </script>
  
  <style>
  /* Your home page CSS */
  .content{
    background-color: #ffffff;
    height: 100vh;
  }
  .btns {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
  .btn {
  width: 330px;
  height: 80px;
  margin: 10px;
  background-color: #65C8FF;
  display: flex;
  justify-content: left;
  color: #ffffff;
  font-size: 24px;
  align-items: center;
  font-size: 20px;
  padding-left: 30px;

  border-radius: 10px;
}
  .btn span {
  padding-left: 200px;

}
  .btn span image {
  width: 8px;
  height: 12px;
  padding: 10px;
  padding-left: 12px;
  padding-right: 12px;
  background-color: #ffffff;
    border-radius: 22px;


}
.imgs swiper{
  height: 200px;
  padding: 20px;
  border-radius: 10px;

}
.imgs swiper-item{
  border-radius: 10px;
  border: ;
}

  </style>
  