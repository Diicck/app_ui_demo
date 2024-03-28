<script>
export default {
  methods:{
    navigateToXinzeng() {
      uni.navigateTo({
        url: '/pages/booking/guahao/lianxiren/xinzeng/xinzeng' // 新增联系人
      })
    }
  }

}
</script>

<template>
  <view class="content">
    <view class="btns">
      <view class="btn02">
        <span class="text01">李文山</span>
        <span class="text01">188568956*9</span>
        <view class="btn02 btn02-right">
        <span>
          <image
              src="@/static/jiantou.png"
              mode="scaleToFill"
          />
</span>

        </view>
      </view>
      <view class="btn02">
        <span class="text01">李文山</span>
        <span class="text01">188568956*9</span>
        <view class="btn02 btn02-right">
        <span>
          <image
              src="@/static/jiantou.png"
              mode="scaleToFill"
          />
</span>

        </view>
      </view>
      <view class="btn02">
        <span class="text01">李文山</span>
        <span class="text01">188568956*9</span>
        <view class="btn02 btn02-right">
        <span>
          <image
              src="@/static/jiantou.png"
              mode="scaleToFill"
          />
</span>

        </view>
      </view>
      <view class="btn03" @click="navigateToXinzeng">
        新增联系人

      </view>

    </view>
  </view>
</template>

<style>
.btn02 .text01{
  width: 200px;
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

.btn02 {
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

/* 按钮内文本 */
.btn02 span {
  width: 100px; /* 控制文本宽度，避免文本溢出 */
}

.text01 {
  font-weight: bold; /* 加粗字体 */
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

.btn03 {
  position: absolute;
  bottom: 0;
  margin-bottom: 20px;
  width: 80%;
  background-color: #216eff;
  display: flex;
  align-items: center;
  color: white;
  border-radius: 10px;
  font-size: 16px;

  padding: 10px 0;
  justify-content: center; /* 调整对齐方式 */
}



</style>