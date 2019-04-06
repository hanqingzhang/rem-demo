<template>
<div>
  <div class="header">
    <ul class="header-content">
      <li class="header-item">新闻</li>
      <li class="header-item">新闻</li>
      <li class="header-item">新闻</li>
      <li class="header-item">新闻</li>
      <li class="header-item">新闻</li>
    </ul>
  </div>
  <div class="banner-content">
    <img src="./styles/pic4.jpg" class="banner">
    <p class="banner-title">2019年度重大新闻</p>
    
  </div>
  <div class="news-content">
    <ul>
      <li class="news-item">
        <div class="item-inner">
          <!--item-inner为了实现底部的线-->
          <img src="./styles/pic4.jpg" class="news-img">
          <p class="news-title">大V领卡少女那架飞机就放到出差电风扇反倒是
          </p>
          <span class="time">1小时前</span>
          <span class="num">9</span>
        </div>
      </li>
      <li class="news-item">
        <div class="item-inner">
          <!--item-inner为了实现底部的线-->
          <img src="./styles/pic4.jpg" class="news-img">
          <p class="news-title">大V领卡少女那架飞机就放到出差电风扇反倒是
          </p>
          <span class="time">1小时前</span>
          <span class="num">9</span>
        </div>
      </li>
      <li class="news-item">
        <div class="item-inner">
          <!--item-inner为了实现底部的线-->
          <img src="./styles/pic4.jpg" class="news-img">
          <p class="news-title">大V领卡少女那架飞机就放到出差电风扇反倒是
          </p>
          <span class="time">1小时前</span>
          <span class="num">9</span>
        </div>
      </li>
    </ul>
  </div>
</div>
</template>

<script>


export default {
  name: 'App',
 
}
</script>

<style lang="scss">
@function px2rem($px){
  $rem:37.5px;
  @return($px/$rem)+rem;

}
.header{
  height:px2rem(40px);
  width:100%;
  padding-left:px2rem(23px);
  background-color:red;
  .header-item{
    color:#ffcdce;
    font-size:px2rem(16px);
    float:left;
    margin-right:px2rem(20px);
    line-height:px2rem(40px);

    &:nth-child(2){
      color:#fff;
      font-size:px2rem(17px);
    }
  }
}
.banner-content{
  position:relative;
  .banner{
  display:block;
  width:100%;
  height:px2rem(190px);
  
  }
  .banner-title{
    font-size:px2rem(16px);
    position:absolute;
    left:px2rem(10px);
    bottom:px2rem(10px);
  }

}
.news-content{
  .news-item{
    width:100%;
    height:px2rem(90px);
    padding-left:px2rem(15px);
    padding-right:px2rem(15px);
    box-sizing:border-box;
  }
  .item-inner{
    border-bottom:px2rem(1px) solid black;
    height:100%;
    overflow:hidden;
    position:relative;

  }
  .news-img{
    display:block;
    width:px2rem(95px);
    height:px2rem(70px);
    margin-top:px2rem(10px);
    margin-right:px2rem(15px);
    float:left;
  }
  .news-title{
    color:black;
    font-size:px2rem(17px);
    margin-top:px2rem(16px);
    line-height:px2rem(20px);
  }
  .time{
    position:absolute;
    left:px2rem(105px);
    bottom:px2rem(17px);
    font-size:px2rem(12px);
    color:grey;
  }
  .num{
    position:absolute;
    right:px2rem(4px);
    bottom:px2rem(17px);
    font-size:px2rem(12px);
    color:grey;
    &:before{
      content:'';
      display:block;
      position:absolute;
      top:px2rem(-3px);
      left:px2rem(-23px);
      width:px2rem(21px);
      height:px2rem(21px);
      background-img:url('./styles/pic4.jpg');
      background-size:contain;
    }
  }
}


</style>
