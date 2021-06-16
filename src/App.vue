<template>
  <div id="app">
    <el-container>
      <el-header style="height: 100%"><Header /></el-header>
      <el-main>
        <div id="wrapper">
          <Login />
        </div>
        <div id="footer"></div>
      </el-main>
      <el-footer>
        <Footer />
      </el-footer>
    </el-container>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Login from "./components/Login.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Login,
    Footer,
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
header.el-header {
  padding: 0;
}
main.el-main {
  padding: 0;
}
footer.el-footer {
  padding: 0;
}
#wrapper {
  position: absolute;
  width: 100%;
  height: 540px;
  background-image: url("./assets/xiecheng.jpg");
}
h1,
h2,
h3,
h4,
h5,
input {
  font-weight: 400;
  font-family: "Microsoft YaHei", SimSun, Tahoma, Verdana, Arial, sans-serif;
}
body a {
  outline: 0;
}
</style>
