<script>
export default {
  methods:{
    Back(){
      //uni.navigateBack()//默认delta:1
      uni.navigateBack({
        delta:1,//返回层数，2则上上页
      })
    }
  }

}
</script>

<template>
  <view class="content">
    <view class="btns">
      <view class="btn02">
        <span class="text01">姓名</span>
        <view class="btn02 btn02-right">
        <span>
          李文山
</span>

        </view>
      </view>
      <view class="btn02">
        <span class="text01">性别</span>
        <view class="btn02 btn02-right">
        <span>
          男
</span>
          <image
              src="@/static/jiantou.png"
              mode="scaleToFill"
          />

        </view>
      </view>
      <view class="btn02">
        <span class="text01">年龄</span>
        <view class="btn02 btn02-right">
        <span>
          18
</span>

        </view>
      </view>
      <view class="btn02">
        <span class="text01">电话</span>
        <view class="btn02 btn02-right">
        <span>
          188568956*9
</span>


        </view>
      </view>
      <view class="btn02">
        <span class="text01">基础病</span>
        <view class="btn02 btn02-right">
        <span>
          无
</span>


        </view>
      </view>
      <view class="btn02">
        <span class="text01">过敏史</span>
        <view class="btn02 btn02-right">
        <span>
          妹妹
</span>


        </view>
      </view>
      <view class="btn02">
        <span class="text01">是否残疾</span>
        <view class="btn02 btn02-right">
        <span>
          否
</span>

        </view>
      </view>

      <view class="btn03" @click="Back">
        保存

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