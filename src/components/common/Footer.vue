<template>
  <!-- 底部开始 -->
  <div class="footer">
    <ul>
      <li v-for="(item, index) in footerList" :key="index">
        <router-link to="">{{ item }}</router-link
        >|
      </li>
    </ul>
  </div>
  <!-- 底部结束 -->
</template>
<script>
export default {
  name: "Footer",
  data() {
    return {
      footerList: [
        "首页",
        "关于我们",
        "联系我们",
        "商城公告",
        "帮助中心",
        "支付中心",
        "客服中心",
        "购尚商城版权所有",
        "粤ICP备17034460119"
      ]
    };
  }
};
</script>
<style scoped>
.footer {
  width: 100%;
  height: 60px;
  background: #f5f5f5;
  border-top: 1px solid #ccc;
  position: absolute;
  bottom: 0;
}
.footer ul {
  padding: 0;
  flex: auto;
  display: inline-block;
  margin: 0 auto;
  height: 100%;
}
.footer ul li {
  line-height: 60px;
  float: left;
  color: #999;
  list-style: none;
}
.footer ul li a {
  padding-left: 10px;
  padding-right: 10px;
  font-size: 14px;
}
</style>
