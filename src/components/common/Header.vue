<template>
  <div class="gs-quick-menu">
    <!-- <img alt="SequnceE" src="../../assets/logo.png" /> -->
    <div class="container">
      <!-- 头部左边 -->
      <div class="gs-profile">
        <span><router-link to="/">首页</router-link></span>
        <span><router-link to="/About">关于我们</router-link></span>
      </div>
      <!-- 头部右边 -->
      <!-- <ul class="gs-nav">
        <li class="gs-nav-item">
          <router-link class="gs-link" to="/order">我的订单</router-link>
        </li>
        <li class="gs-nav-item">
          <router-link class="gs-link" to="/cart">
            <i class="fa fa-shopping-cart"></i> 购物车
          </router-link>
        </li>
        <li class="gs-nav-item">
          <span class="gs-link gs-forbid">收藏夹</span>
        </li>
        <li class="gs-nav-item">
          <span class="gs-link gs-forbid">商家入口</span>
        </li>
      </ul> -->
    </div>
  </div>
</template>
<script>
export default {
  name: "Header"
};
</script>
<style scoped>
.container {
  /* width: 80%; */
  height: 100%;
  margin: 0 auto;
  display: inline-grid; /* 剧中 */
}
.gs-link {
  color: #999;
  text-decoration: none;
  outline: none;
}
.gs-forbid {
  cursor: not-allowed;
}
.gs-menu-bg {
  position: absolute;
  width: 10%;
  height: 40px;
  background-color: #f2f2f2;
  border-bottom: 1px solid #e5e5e5;
}

.gs-header {
  width: 1120px;
  margin-left: auto;
  margin-right: auto;
}
.gs-quick-menu {
  position: relative;
  font-size: 16px;
  color: azure;
  background-color: #373234;
  height: 50px;
}
.gs-quick-menu img {

}
.gs-profile span a {
  /* background-color: palegreen; */
  padding-left: 15px;
  padding-right: 15px;

  color: #c8d7d2;

  text-decoration: none;
}
.gs-profile {
  display: inline-block;
  /* line-height: 30px; */
  line-height: 300%;

  cursor: pointer;
  float: left;
}
/* .gs-profile a:active {
  color: bisque;
} */
.gs-profile a:hover {
  color: #f4f2fd;
  padding-bottom: 3px;
  border-bottom: #d84339 8px solid;
}
/* .gs-profile a:focus {
  color: azure;
} */
/* .gs-profile a:visited {
  color: violet;
} */
/* .gs-nav {
  display: inline-block;
  line-height: 30px;
  list-style: none;
  margin: 0;
  float: right;
} */
/* .gs-nav-item {
  margin-left: 12px;
  display: inline-block;
} */
</style>
