<template>
  <div id="header">
    <div class="header">
      <h1 class="ctriplogo_login ctriplogoindex">
        <a href="http://www.ctrip.com" title="携程旅行网"></a>
      </h1>
    </div>
    <div class="tips-security">
      <i class="icon-warn"></i
      >依据《网络安全法》，为保障您相关功能的正常使用，账号需绑定手机，如您未绑定则登录后会引导您操作绑定。
      新版<a
        href="https://contents.ctrip.com/huodong/privacypolicypc/index?type=1"
        target="_blank"
        >《隐私政策》</a
      >已上线，感谢您的支持。
    </div>
  </div>
</template>

<script>
export default {
    name:'Header',
};
</script>

<style>
.header {
  width: 980px;
  height: 90px;
  margin-left: auto;
  margin-right: auto;
  padding: 0 10px;
}
.ctriplogo_login {
  float: left;
  width: 203px;
  padding-top: 22px;
  margin-right: 10px;
}
.ctriplogo_login a {
  display: block;
  width: 100%;
  height: 34px;
  overflow: hidden;
  text-indent: -999em;
  background: url(//pic.c-ctrip.com/platform/online/login/c_logo2020.png)
    no-repeat;
  background-size: 100% 100%;
}

.tips-security {
  width: 100%;
  padding: 7px 0;
  margin-top: -10px;
  line-height: 16px;
  background: #fffcd8;
  font-family: "Microsoft yahei";
  font-size: 12px;
  color: #666;
  text-align: center;
  vertical-align: middle;
}
.tips-security .icon-warn {
  margin-right: 6px;
  vertical-align: middle;
}
a {
  color: #666;
  text-decoration: none;
  outline: 0;
}
</style>