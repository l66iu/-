<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="css\base初始化.css">
    <link rel="stylesheet" href="css\normalize.css">
   <style>
       body {
    max-width: 540px;
    min-width: 320px;
    margin: 0 auto;
    font: normal 14px/1.5 Tahoma, "Lucida Grande", Verdana, "Microsoft Yahei", STXihei, hei;
    color: #000;
    background: #f2f2f2;
    overflow-x: hidden;
    -webkit-tap-highlight-color: transparent;
}


.serch_index{
    display: flex;
    position: fixed;
    top: 0;
    left: 50%;
    transform: translateX(-50%);
    width: 100%;
    max-width: 540px;
    min-width: 320px;
    height: 44px;
    background-color: #f6f6f6;
    border-top: 1px solid #ccc;
    border-bottom: 1px solid #ccc;
}
.serch{
    position: relative;
    height: 26px;
    flex: 1;
    border: 1px solid #ccc;
    margin: 7px 10px;
    border-radius: 4px;
    box-shadow: 0px 3px 4px rgb(0,0,0,0.3);  
    line-height: 24px;
    font-size: 12px;
    color: #666;  
    padding-left: 27px;
}
.serch::before{
   position: absolute;
   top: 7px;
   left: 5px;
    content: "";
    height: 15px;
    width: 15px;
    background: url(../images/sprite.png) no-repeat -60px -280px;
    background-size: 104px auto;

}
.user{
    width: 44px;
    height: 44px;
    font-size: 12px;
    text-align: center;
    color: #2eaae0;
}
.user::before{
    content: "";
    display: block;
    width: 23px;
    height: 23px;
    background: url(../images/sprite.png) -58px -194px;
    background-size: 104px auto;
    margin: 2px 10px 0px 10px;
   
}
.fous{
    margin-top: 44px;
}
.fous img{
    width: 100%;
}
.nav{
    display: flex;
    height: 64px;
    background-color: #fff;
    border-radius: 8px;
    overflow: hidden;
    margin: 3px 4px;
}
.nav li{
    flex: 1;
    height: 100%;
}
.nav a{
    display: flex;

    flex-direction: column;
    align-items: center;
    font-size: 12px;
    color:#222

}
.nav .name{
    width: 32px;
    height: 32px;
    background: url(../images/localnav_bg.png) no-repeat;
    background-size: 32px auto;
    margin-top: 8px;
}
.nav li:nth-child(2) .name{
    width: 32px;
    height: 32px;
    background: url(../images/localnav_bg.png) no-repeat 0 -64px;
    background-size: 32px auto;
    margin-top: 8px;
}
.nav li:nth-child(3) .name{
    width: 32px;
    height: 32px;
    background: url(../images/localnav_bg.png) no-repeat 0 -96px;
    background-size: 32px auto;
    margin-top: 8px;
}
.nav li:nth-child(4) .name{
    width: 32px;
    height: 32px;
    background: url(../images/localnav_bg.png) no-repeat 0 -128px;
    background-size: 32px auto;
    margin-top: 8px;
}
.nav li:nth-child(5) .name{
    width: 32px;
    height: 32px;
    background: url(../images/localnav_bg.png) no-repeat 0 -32px;
    background-size: 32px auto;
    margin-top: 8px;
}
.navs{
    border-radius: 4px;
    overflow: hidden;
    margin: 3px 4px;
}
.navs_a{
    display: flex;
    height: 88px;
   
}
.navs_aa{
    flex: 1;
    display: flex;
    flex-direction: column;
}
.navs_aa a{
    flex: 1;
    text-align: center;
    line-height: 44px;
}
.navs_aa a:nth-child(n+2){
    border-top: 1px solid #ccc;
}
.navs_a:nth-child(2){
    margin: 3px 0;
}
.navs_aa:nth-child(-n+2){
    border-right: 1px solid #ccc;
}
.navs_aa:nth-child(1) a{
    background: url(../images/hotel.png) no-repeat bottom;
    background-size: 121px auto;
  background-position: center bottom;
}
.navs_a:nth-child(1){
    background: -webkit-linear-gradient(left ,#fa5a55,#fa994d);
}
.navs_a:nth-child(2){
    background: -webkit-linear-gradient(left ,#44c8f1,#3591e8);
}
.navs_a:nth-child(3){
    background: -webkit-linear-gradient(left ,#71e98b,#3fd128);
}



.navb{
    display: flex;
    flex-wrap: wrap;
    border-radius: 4px;
    margin: 3px 4px;
    background-color: #fff;
}
.navb li{
    flex: 20%;
}
.navb li a{
    display: flex;
    flex-direction: column;
    text-align: center;
    align-items: center;

}
.bj{
    width: 28px;
    height: 28px;
    background: url(../images/subnav-bg.png) no-repeat;
    background-size: 28px auto;
    margin-top: 10px;
}


.hot{
    margin: 3px 4px;
    border-top: 1px solid #ccc;
    background-color: #fff;
    background-color: #fff;
}
.hot_hd{
    position: relative;
    padding-top: 20px;
  width:100%;
  height: 44px;
  border-bottom: 1px solid #ccc;

}
.hot_hd h2{
    margin-left: 7px;
    width: 79px;
    height: 15px;
    background: url(../images/hot.png) no-repeat 0 -20px;
    background-size: 79px auto;
    text-indent: 999px;
}
.hot_hd a{
    position: absolute;
    top: 12px;
    right: 10px;
   color: #fff;
    border-radius: 15px;
    padding: 3px 20px 3px 10px;
    background: -webkit-linear-gradient(left, #FF506C, #FF6BC6);
}

.row{
    display: flex;
    border-bottom: 1px solid #ccc;
}
.row a{
    flex: 1;
}
.row a img{
   width: 100%;
}

.row a:nth-child(1){
    border-right: 1px solid #ccc;
}

.app{
    display: flex;
    justify-content: space-around;
    margin: 20px 12px;
        
}
.app a{
 display: flex;
    justify-content: center;
    align-items: center;
    height: 30px;
    border: 1px solid #999;
    border-radius: 4px;
    min-width: 100px;
}
.xinxi{
    text-align: center;
}
.xinxi a{
    margin: 10px 40px;
}
.xinxi p{
    padding-top: 10px;
}

.app a span::before{
    margin-right: 4px;
    font-family: 'icomoon';
    content: "\e9c7";
    font-size: 10px;
}

    </style>
</head>
<body>
    <!-- 搜索 -->
    <div class="serch_index">
        <div class="serch">搜索:目的地/住宿/飞机</div>
        <a href="#" class="user">我的</a>
    </div>
    <!-- 焦点图 -->
    <div class="fous">
        <a href="#"><img src="upload\focus.jpg" alt=""></a>
    </div>
    <!-- 局部导航栏 -->
    <ul class="nav">
     <li>
        <a href="#">
          <span class="name"></span>
          <span>景点·玩乐</span>
        </a>
</li>
     <li> <a href="#">
        <span class="name"></span>
        <span>携程·酒店</span>
      </a></li>
     <li> <a href="#">
        <span class="name"></span>
        <span>星级·餐厅</span>
      </a></li>
     <li> <a href="#">
        <span class="name"></span>
        <span>携程·导航</span>
      </a></li>
     <li> <a href="#">
        <span class="name"></span>
        <span>景点·玩乐</span>
      </a></li>
    </ul>
    <!-- 导航栏 -->
    <div class="navs">

      <div class="navs_a">
        <div class="navs_aa"><a href="#">海外酒店</a></div>
        <div class="navs_aa"><a href="#">海外酒店</a><a href="#">特价酒店</a></div>
        <div class="navs_aa"><a href="#">海外酒店</a><a href="#">特价酒店</a></div>
      </div>

      <div class="navs_a">
        <div class="navs_aa"><a href="#">海外酒店</a></div>
        <div class="navs_aa"><a href="#">海外酒店</a><a href="#">特价酒店</a></div>
        <div class="navs_aa"><a href="#">海外酒店</a><a href="#">特价酒店</a></div>
      </div>

      <div class="navs_a">
        <div class="navs_aa"><a href="#">海外酒店</a></div>
        <div class="navs_aa"><a href="#">海外酒店</a><a href="#">特价酒店</a></div>
        <div class="navs_aa"><a href="#">海外酒店</a><a href="#">特价酒店</a></div>
      </div>
    </div>
    <!-- 局部导航栏2 -->
    <ul class="navb">
      <li><a href="#"><span class="bj"></span><span>无线wifi</span> </a></li>
      <li><a href="#"><span class="bj"></span><span>无线wifi</span> </a></li>
      <li><a href="#"><span class="bj"></span><span>无线wifi</span> </a></li>
      <li><a href="#"><span class="bj"></span><span>无线wifi</span> </a></li>
      <li><a href="#"><span class="bj"></span><span>无线wifi</span> </a></li>
      <li><a href="#"><span class="bj"></span><span>无线wifi</span> </a></li>
      <li><a href="#"><span class="bj"></span><span>无线wifi</span> </a></li>
      <li><a href="#"><span class="bj"></span><span>无线wifi</span> </a></li>
      <li><a href="#"><span class="bj"></span><span>无线wifi</span> </a></li>
      <li><a href="#"><span class="bj"></span><span>无线wifi</span> </a></li>
    </ul>
    <!-- 热门活动 -->
    <div class="hot">
      <div class="hot_hd">
        <h2></h2>
        <a href="#">获取更多福利</a>
      </div>
      <div class="row">
        <a href="#"><img src="upload\pic1.jpg" alt=""></a>
        <a href="#"><img src="upload\pic2.jpg" alt=""></a>
      </div>
      <div class="row"> 
        <a href="#"><img src="upload\pic3.jpg" alt=""></a>
        <a href="#"><img src="upload\pic4.jpg" alt=""></a>
      </div>
      <div class="row"> 
        <a href="#"><img src="upload\pic5.jpg" alt=""></a>
        <a href="#"><img src="upload\pic6.jpg" alt=""></a>
      </div>
    </div>
    <!--  信息和版权-->
    <div class="app">
      <a href="#">   
        <span>电话预订</span>
      </a>
      <a href="#">
        <span>APP下载</span>
      </a>
    </div>
    <div class="xinxi">
      <a href="#">网站地图</a>
      <a href="#">电脑版</a>
      <p>2022携程旅行&nbsp;沪备案2013100@</p>
      <p>20555</p>
    </div>
</body>
</html>

