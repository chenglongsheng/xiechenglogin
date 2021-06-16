<template>
  <div id="login">
    <el-card class="box-card">
      <div slot="header" class="clearfix">
        <span id="title">携程账号登录</span>
        <el-button style="float: right; padding: 3px 0" type="text"
          >手机号查单</el-button
        >
      </div>
      <div id="loginContent">
        <el-input
          id="username"
          class="text item"
          v-model="user.username"
          placeholder="国内手机号码/用户名/邮箱/卡号"
        ></el-input>
        <el-input
          id="password"
          class="text item"
          v-model="user.password"
          placeholder="登录密码"
          show-password
        ></el-input>
      </div>
      <div class="login-set">
        <label class="auto-login"
          ><input
            type="checkbox"
            checked="checked"
            id="normal30day"
          />30天内自动登录</label
        >
        <a href="" class="login-entry-dynamic">手机动态密码登录</a>
      </div>

      <div id="loginSubmit">
        <el-button id="submitButton" @click="submitButton">登录</el-button>
      </div>
      <p class="agreement-list">
        登录即代表您同意我们的<a
          href="https://contents.ctrip.com/huodong/privacypolicypc/index?type=0"
          class="serviceAgreement"
          target="_black"
          >服务协议</a
        >和<a
          href="https://contents.ctrip.com/huodong/privacypolicypc/index?type=1"
          class="privacyPolicy"
          target="_black"
          >隐私政策</a
        >
      </p>
      <div class="lg_weblogin" id="loginbanner" style="display: block">
        <div class="login-about">
          <a href="javascript:;" id="overseas_login">境外手机</a
          ><span class="sep">|</span
          ><a
            href="https://ct.ctrip.com/#ctm_ref=ctriplogin"
            class="companylogin"
            >公司客户</a
          ><span class="sep">|</span
          ><a
            class="cardlogin"
            target="_self"
            href="javascript:;"
            style="display: none"
            >合作卡</a
          ><span class="sep" id="cardloginsep" style="display: none">|</span
          ><a class="fuli" target="_self" href="https://b.ctrip.com/">携程通</a
          ><a
            href="https://passport.ctrip.com/user/reg/home"
            class="free-regist"
            target="_black"
            >免费注册</a
          >
        </div>
        <div class="login-other">
          <a href="" class="iconfont icon-alipay">支付宝</a><a href="">QQ</a
          ><a href="" class="iconfont icon-baidu">百度</a
          ><a href="" class="iconfont icon-sina">新浪微博</a
          ><a href="" class="iconfont icon-wechat">微信</a
          ><a href="" style="display: none" class="icon-163">网易</a
          ><a href="" class="icon-renren" style="display: none">人人网</a>
        </div>
      </div>
    </el-card>
  </div>
</template>

<script>
export default {
  name: "Login",
  //   props: {
  //     msg: "minduansuid"
  //   },
  data() {
    return {
      user: {
        username: "",
        passwoed: "",
      },
    };
  },
  methods: {
    submitButton() {
      if (user.username == null || password == null) {
        alert("用户名或密码不能为空");
      }
    },
  },
};
</script>

<style>
.icon {
  width: 1em;
  height: 1em;
  vertical-align: -0.15em;
  fill: currentColor;
  overflow: hidden;
}
#title {
  position: relative;
  padding-bottom: 16px;
  font-size: 18px;
  color: #111;
  line-height: 1;
  font-family: PingFangSC-Medium, "Microsoft YaHei", SimSun, Tahoma, Verdana,
    Arial, sans-serif;
}
.login-set {
  margin: 4px 0 13px;
}
.auto-login {
  line-height: 1;
}
.login-entry-dynamic {
  float: right;
  color: #666;
}

#submitButton {
  display: block;
  margin: 0 auto;
  background-color: #ff9a14;
  color: white;
  border-color: #ff9a14;
  width: 340px;
}
.text {
  font-size: 14px;
}

.item {
  margin-bottom: 18px;
}
.agreement-list {
  margin-top: 5px;
  color: #999;
  line-height: 12px;
  text-align: center;
}

.lg_weblogin {
  margin-top: 52px;
}
.lg_weblogin .login-about {
  margin-bottom: 20px;
  line-height: 1;
}
.lg_weblogin .login-other {
  text-align: left;
  margin-right: -18px;
}
.lg_weblogin .login-about .sep {
  padding: 0 10px;
  color: #ccc;
}
.lg_weblogin .login-about a.free-regist {
  float: right;
  color: #3882e5;
}
.lg_weblogin .login-other a {
  margin-right: 18px;
}

.clearfix:before,
.clearfix:after {
  display: table;
  content: "";
}
.clearfix:after {
  clear: both;
}

.box-card {
  width: 380px;
  position: relative;
  top: 60px;
  left: 1000px;
  /* margin-top: 60px; */
}
body {
  font: 12px/1.5 PingFangSC-Regular, "Microsoft YaHei", SimSun, Tahoma, Verdana,
    Arial, sans-serif;
  color: #666;
  background-color: #fff;
}
</style>