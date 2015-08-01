### 导航滑动插件

***

~~~html
<style>
.nav-box {
position: relative;
}

ul {
padding: 0;
}

ul a {
  text-decoration: none;
}

.nav-box ul li {
list-style: none;
float: left;
padding: 0 12px;
}

.nav-box ul li:first-child {
padding: 0 12px 0 0;
}

.nav-box .nav-line {
position: absolute;
bottom: -35px;
height: 3px;
line-height: 10px;
font-size: 0;
}
</style>
<div class="nav-box">
  <ul>
      <li><a href="#">选择套餐</a></li>
      <li id="order"><a href="#">我的订单</a></li>
      <li id="coupon"><a href="#">我的优惠券</a></li>
      <li id="car"><a href="#">我的车库</a></li>
      <li id="profile" class="cur"><a href="#">个人资料</a></li>
  </ul>
  <div class="nav-line"></div>
</div>
~~~

~~~javascript
$('.nav-box').navBar(jQuery.parseJSON('{"background-color" : "#FFB500"}'));
~~~