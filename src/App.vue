<template>
  <div id="app">
    <!-- 卡片组件 -->
    <el-card class="login-card">
      <!-- 登录表单 -->
      <el-form style="margin-top: 50px" :model="loginForm">
        <el-form-item>
          <el-input
            v-model="loginForm.mobile"
            placeholder="请输入手机号"
          ></el-input>
        </el-form-item>
        <el-form-item>
          <el-input
            v-model="loginForm.password"
            placeholder="请输入密码"
          ></el-input>
        </el-form-item>
        <el-form-item>
          <el-button type="primary" style="width: 100%">登录</el-button>
        </el-form-item>
      </el-form>
    </el-card>
  </div>
</template>

<script>
export default {
  name: 'App',
  data() {
    return {
      // 表单数据
      loginForm: {
        mobile: '',
        password: '',
      },
    };
  },
};
</script>

<style>
#app {
  width: 100%;
  height: 100vh;
  background-color: pink;
  display: flex;
  justify-content: center;
  align-items: center;
}
.login-card {
  width: 440px;
  height: 300px;
}
</style>
