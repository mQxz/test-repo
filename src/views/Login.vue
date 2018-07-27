<template>
  <div class="container">
    <div class="login">
      <h1 class="title">哗啦啦老板通</h1>
      <el-input v-model="phone" placeholder="手机号"></el-input>
      <div class="verify-box">
        <el-input v-model="verify" placeholder="验证码"></el-input>
        <el-button type="primary">获取验证码</el-button>
      </div>
      <el-button type="primary">登录</el-button>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'login',
    data() {
      return {
        phone: '',
        verify: ''
      }
    }
  }
</script>

<style lang="scss" scoped>
  .container {
    padding: 100px 0 0;
    width: 100%;
    height: 100%;
    background-color: #26374C;
  }

  .login {
    margin: 0 auto;
    padding: 30px;
    width: 340px;
    height: 300px;
    border-radius: 8px;
    background-color: rgba(255, 255, 255, 0.1);

    .title {
      font-size: 30px;
      text-align: center;
      color: #fff;
    }

  }
</style>
