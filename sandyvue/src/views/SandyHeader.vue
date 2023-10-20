<template>
    <div>
      <el-row>
        <el-col :span="12"><div class="header1"></div></el-col>
        <el-col :span="12"><div class="header2"></div></el-col>
        <el-col :span="3"><div class="h"><el-input placeholder="想找些什么？" prefix-icon="el-icon-search" v-model="input1"></el-input></div></el-col>
        <el-col :span="1"><div><el-link type="info" underline="false" class="a">首页</el-link></div></el-col>
        <el-col :span="1"><div class="e">|</div></el-col>
        <el-col :span="1"><div><el-link type="info" underline="false" class="b">热点</el-link></div></el-col>
        <el-col :span="1"><div class="f">|</div></el-col>
        <el-col :span="1"><div><el-link type="info" underline="false" class="c">视频</el-link></div></el-col>
        <el-col :span="1"><div class="g">|</div></el-col>
        <el-col :span="1"><div><el-link type="info" underline="false" class="d">收藏</el-link></div></el-col>
      </el-row>
      <el-row>
        <router-view/>
    </el-row>
    </div>
</template>

<script>
export default {
  data() {
    return {
      input1: '',
    }
  }
}
</script>

<style>
.header1{
  background-color: #fff4c5;
  background-image: url(../../image/2.png);
  background-repeat: no-repeat;
  background-position: 400px -30px;
  background-size:21%;
  height: 150px;
}
.header2{
  background-color: #fff4c5;
  background-image: url(../../image/2.png);
  background-repeat: no-repeat;
  background-position: 100000px -30px;
  background-size:21%;
  height: 150px;
}
.a{
position: absolute;
left: 69%;
top: 50%;
transform: translate(-50%, -50%);
height: 150px;
}
.b{
position: absolute;
left: 75%;
top: 50%;
transform: translate(-50%, -50%);
height: 150px;
}
.c{
position: absolute;
left: 81%;
top: 50%;
transform: translate(-50%, -50%);
height: 150px;
}
.d{
position: absolute;
left: 87%;
top: 50%;
transform: translate(-50%, -50%);
height: 150px;
}
.e{
position: absolute;
left: 72%;
top: 95%;
transform: translate(-50%, -50%);
height: 150px;
}
.f{
position: absolute;
left: 78%;
top: 95%;
transform: translate(-50%, -50%);
height: 150px;
}
.g{
position: absolute;
left: 84%;
top: 95%;
transform: translate(-50%, -50%);
height: 150px;
}
.h{
position: absolute;
left: 59%;
top: 86%;
transform: translate(-50%, -50%);
height: 150px;
}
</style>