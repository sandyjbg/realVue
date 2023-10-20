<template>
  <div>
    <el-row>
      <el-col :span="12"><div class="login4"></div></el-col>
      <el-col :span="6"><div class="login5">
        <el-row>
          <el-col :span="24"><div class="login">登  录</div></el-col>
        </el-row>
        <el-row>
            <el-col :span="24"><div class="zhanghaomima">
              <el-input placeholder="请输入账号" prefix-icon="el-icon-user" v-model="input"></el-input>
              <el-input placeholder="请输入密码" prefix-icon="el-icon-lock" v-model="input"></el-input>
            </div></el-col>
        </el-row>
        <el-row>
          <el-col :span="24"><div class="denglu"><el-button type="warning" style="width:260px" @click="blog">登录</el-button></div></el-col>
        </el-row>
        <el-row>
          <el-col :span="12"><div class="login6"><el-link type="warning">忘记密码？</el-link></div></el-col>
        </el-row>
        <el-row>
          <el-col :span="11"><div class="login7">还没有账号？</div></el-col>
          <el-col :span="4"><div class="login8"><el-link type="warning" :underline="true">注册</el-link></div></el-col>
        </el-row>
      </div></el-col>
    </el-row>
  </div>
</template>

<script>
export default {
  data() {
    return {
      input: ''
    }
  },
methods: {
  blog()
      {
        this.$router.push({path:'/SandyBlog'})
      }
}
}
</script>

<style>
.login{
  color:rgb(255, 187, 0);
  font-family: 华文宋体;
  font-weight: bolder;
  font-size: 3em;
  margin: 50px auto;
}
.zhanghaomima{
 width:70%;
 margin:0 auto 40px auto;
}
.denglu{
  width:70%;
  margin:0px auto 30px auto;
}
.login4{
  background-image: url(../../image/4.png);
  background-repeat: no-repeat;
  min-height:500px;
  background-position: 460px -30px;
}
.login6{
  margin:0px auto 15px 0px;
}
.login7{
  margin:0px auto 70px 40px;
}
.login8{
  margin:0px 30px 70px 0px;
}
.login4{
  margin:100px 0px 0px 0px;
}
.login5{
  background-color: #fffbeb;
  margin:100px 100px 0px 0px;
  /* box-shadow: 0px 1px 0px 1px black; */
}
body{
  background-color: #fffbeb;
}
</style>