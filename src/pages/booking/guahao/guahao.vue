<script>
export default {
  methods:{
    navigateToXianxiren() {
      uni.navigateTo({
        url: '/pages/booking/guahao/lianxiren/lianxiren' // 选择联系人
      })
    }
  }

}
</script>

<template>
  <view class="content">
    <view class="btns">
      <view class="btn02" @click="navigateToXianxiren">
        <span class="text01">选择联系人</span>
        <view class="btn02 btn02-right">
        <span>
          名字
</span>
          <image
              src="@/static/jiantou.png"
              mode="scaleToFill"
          />
        </view>
      </view>
      <view class="btn02">
        <span class="text01">
          意向医院
</span>

        <view class="btn02 btn02-right">
        <span>
          首都附属医院
</span>
        </view>
      </view>
      <view class="btn02">
        <span class="text01">
          意向科室
</span>

        <view class="btn02 btn02-right">
        <span>
          骨科
</span>
        </view>
      </view>
      <view class="btn02">
        <span class="text01">
          意向专家
</span>

        <view class="btn02 btn02-right">
        <span>
          王晓霞
</span>
        </view>
      </view>
      <view class="btn02">
        <span class="text01">
          就诊时间
</span>

        <view class="btn02 btn02-right">
        <span>
          2024/03/22 17:03
</span>
          <image
              src="@/static/jiantou.png"
              mode="scaleToFill"
          />
        </view>
      </view>
      <view class="btn">
        <span class="text01">其他服务</span>
        <view class="btn02 btn02-right">
          <view class="service-option">需要陪同</view>
          <view class="service-option">需要轮椅</view>

          <view class="service-option">需要住院</view>
          <view class="service-option">需要陪同</view>
        </view>
      </view>
      <view class="btn">

        <span class="text01">备注</span>
        <span class="text02">111111111111</span>

      </view>
      <view class="btn03">

        <span class="text01">
          订单金额<span>10</span>元
</span>

        <view class="btn03 btn02-right">
        <span>
          支付
</span>
        </view>


      </view>

    </view>
  </view>
</template>

<style>
.btn02 .text01{
  width: 200px;
}
.btn03 .text01{
  width: 200px;
  color: white;
  font-weight: normal;
}
.btn03 .text01 span{
  width: auto;
  color: white;
  font-size: 20px;
  font-weight: normal;
}
.btn03 .btn02-right span{
  width: auto;
  padding: 5px 20px;
  background: #ffffff;
  border-radius: 15px;
  font-weight: bold;
}
.content{
  background-color: #F1F6FC;
  height: 100vmax;
}

.btns {
  font-family: "PingFang SC",sans-serif;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

/* 通用按钮样式 */
.btn, .btn01, .btn02 {
  width: 80%;
  background-color: #ffffff;
  display: flex;
  align-items: center;
  padding-left: 10px;
  border-radius: 10px;
  font-size: 16px;
  margin: 10px;
  justify-content: left; /* 调整对齐方式 */
}
.btn03 {
  width: 80%;
  background-color: #216eff;
  display: flex;
  align-items: center;
  padding-left: 10px;
  border-radius: 10px;
  font-size: 16px;
  margin: 10px;
  justify-content: left; /* 调整对齐方式 */
}

/* 特定于.btn的样式，用于区分大按钮 */
.btn {
  height: 150px; /* 大按钮的高度 */
  align-items: flex-start; /* 调整子项对齐方式 */
}

/* 按钮内文本 */
.btn span, .btn02 span {
  width: 100px; /* 控制文本宽度，避免文本溢出 */
}

.text01 {
  font-weight: bold; /* 加粗字体 */
}
.btn .text01 {
  margin-top: 10px;
  font-weight: bold; /* 加粗字体 */
}
.btn .text02 {
  margin-top: 10px;
  color: #8f8f94;
}

.btn02-right {

  justify-content: flex-end;
  padding-right: 10px;
}

.btn02-right span {
  text-align: right;
  width: auto /* 为 "btn02-right" 内的文本调整宽度 */
}

.btn02-right image {
  padding-left: 5px;
  width: 8px;
  height: 12px;
}

/* 调整具有特殊功能的按钮的样式 */
.btn .btn02 {
  width: 180px;
  height: 110px; /* 高度与.btn相同 */
  align-items: flex-start;
}
.btn .btn02-right{
  display: flex;
  flex-wrap: wrap;
}

/* 特殊按钮内部view的样式 */
.btn .btn02 view {

  padding: 0 5px;
  background: #007aff;
  border: 1px solid #4cd964;
  width: auto; /* 自动宽度，根据内容调整 */
  height: auto;
  border-radius: 20px;

}
/* 特殊服务选项按钮样式 */
.service-option {
  margin: 2px;
  padding: 8px 12px; /* 增加内边距以提供更多空间，使文本更易读 */
  background-color: #007aff; /* 明亮的蓝色背景，吸引视线 */
  color: #ffffff; /* 白色文字，以确保对比度和可读性 */
  border: 1px solid #4cd964; /* 使用稍微对比的边框颜色增加美观性 */
  border-radius: 20px; /* 圆角边框，使按钮看起来更友好、更现代 */
  white-space: nowrap; /* 防止文本换行 */
  display: inline-block; /* 允许元素依照内容自动调整宽度 */
  text-align: center; /* 文本居中显示 */
  cursor: pointer; /* 鼠标悬停时显示指针，增强交互感 */
}


</style>