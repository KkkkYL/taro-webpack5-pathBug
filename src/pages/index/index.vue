<template>
  <view class="index">
    <text>图片(PNG)↓</text>
    <view class="text-img-box"></view>
    <text>图片(base64)↓</text>
    <view class="text-img2-box"></view>
    <view class="text-font-box">导入的字体包,打包后不生效</view>
  </view>
</template>

<script>
import { ref } from 'vue'
import './index.less'

export default {
  setup () {
    const msg = ref('Hello world')
    return {
      msg
    }
  }
}
</script>

<style lang="less" scoped>
.index {
  .text-img-box {
    width: 300px;
    height: 300px;
    background: url('../../static/test-img.png') no-repeat;
    background-size: contain;
  }
  .text-img2-box {
    width: 300px;
    height: 300px;
    background: url('../../static/test-base64.png') no-repeat;
    background-size: contain;
  }
  .text-font-box {
    font-family: Alimama;
  }
}
</style>