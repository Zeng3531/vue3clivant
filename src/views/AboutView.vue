<template>
  <div class="about">
    <van-button type="primary">主要按钮</van-button>
<van-button type="success">成功按钮</van-button>
<van-button type="default">默认按钮</van-button>
<van-button type="warning">警告按钮</van-button>
<van-button type="danger">危险按钮</van-button>
<van-swipe class="my-swipe" :autoplay="3000" :width="350" indicator-color="white">
  <van-swipe-item>1</van-swipe-item>
  <van-swipe-item>2</van-swipe-item>
  <van-swipe-item>3</van-swipe-item>
  <van-swipe-item>4</van-swipe-item>
</van-swipe>

  </div>
  
</template>
<style lang="scss">
  .about{
    font-size:pxrem(50);
  }
  .my-swipe .van-swipe-item {
    color: #fff;
    font-size: 20px;
    line-height: 3rem;
    text-align: center;
    background-color: #39a9ed;
  }
  .van-swipe-item{
    background-color: red;
    margin:2rem ;
  }
</style>
