<template>
  <div class="login">
    <div class="login">
      <div class="login-card">
        <h3 class="login-card-title">欢迎登录</h3>
        <el-form
          :model="userFrom"
          :rules="rules"
          ref="form"
          class="login-card-form"
          size="small"
        >
          <el-form-item prop="username">
            <el-input placeholder="请输入内容" v-model="userFrom.username">
              <el-button slot="prepend" icon="el-icon-user-solid"></el-button>
            </el-input>
          </el-form-item>

          <el-form-item prop="password">
            <el-input
              type="password"
              placeholder="请输入内容"
              v-model="userFrom.password"
            >
              <el-button slot="prepend" icon="el-icon-lock"></el-button>
            </el-input>
          </el-form-item>
          <!-- <el-from-item> -->
          <el-button @click="login" type="primary" class="width100"
            >登录</el-button
          >
          <!-- </el-from-item> -->
        </el-form>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "Login"
};
</script>