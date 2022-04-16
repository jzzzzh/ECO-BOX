/* eslint-disable */
<template>
  <div class = "home">
    <div class="note" :style ="note">

      <br>
      <div v-if="flag1 == 1">
        <br>
        <div class = "textButton">
          <el-button type="primary"  plain @click="flag1 = 1">具体介绍</el-button>
          <el-button type="primary"  plain @click="flag1 = 2">少儿编程</el-button>
          <el-button type="primary"  plain @click="flag1 = 3">联系我们</el-button>
        </div>
        <h1  class="title" id = "h1highlight1"> AI ECO-BOX 基于物联网的新型智能生态箱 </h1>
        <h3 class="title" id = "h3highlight1">A new intelligent eco box based on Internet of things</h3>
        <div class="detail">
          <img-and-word msg="简介" para="本项目采用计算机控制技术替代人工以控制植物的生长环境，科学运用物联网感应技术，来实现对植物生长过程的实时监测和对温度、湿度、光照等因素的调控，植物创造适宜的生长环境。"></img-and-word>
          <img-and-word msg="原理" para="本项目通过温度传感器、湿度传感器、光照强度传感器等多种传感器获取生态箱内部环境参数的实时数据，运用树莓派进行终端统一智能调控。通过终端系统判断接收的数据是否在正常范围内，若超出正常值范围，则树莓派控制系统开始工作，直到接收的数据达到正常"></img-and-word>
          <img-and-word msg="教育" para="开发以在太空和地外行星进行农业种植为背景的课程体系，让学生在模拟宇宙和行星环境中进行选种育种、无土栽培、智慧农业的过程。 "></img-and-word>
        </div>
      </div>



      <div v-if="flag1 == 2">
        <br>
        <div class = "textButton">
          <el-button type="primary"  plain @click="flag1 = 1">具体介绍</el-button>
          <el-button type="primary"  plain @click="flag1 = 2">少儿编程</el-button>
          <el-button type="primary"  plain @click="flag1 = 3">联系我们</el-button>
        </div>
        <h2  class="title2" id = "h1highlight2"> 少儿编程 </h2>
        <div class="input">
          <el-input
              v-model="textarea"
              :rows="6"
              type="textarea"
              placeholder="Please input"
              clearable
          >
            <template #suffix>
              <el-icon class="el-input__icon"><connection /></el-icon>
            </template>
          </el-input>
        </div>

        <el-button type="primary" round id="upput" size="large" auto-insert-space>    提交您的代码     </el-button>
        <back></back>
      </div>



        <div v-if="flag1 == 3">
          <br>
          <div class = "textButton">
            <el-button type="primary"  plain @click="flag1 = 1">具体介绍</el-button>
            <el-button type="primary"  plain @click="flag1 = 2">少儿编程</el-button>
            <el-button type="primary"  plain @click="flag1 = 3">联系我们</el-button>
          </div>
          <h1  class="title" id = "h1highlight3"> AI ECO-BOX 基于物联网的新型智能生态箱 </h1>
          <h3 class="title" id = "h3highlight3">A new intelligent eco box based on Internet of things</h3>
          <div class="detail">
            <img-and-word url="2" msg="电话" para="17358832218"></img-and-word>
            <img-and-word url="3" msg="邮箱" para="2657246129@qq.com"></img-and-word>
            <img-and-word url="4" msg="地址" para="四川省成都市四川大学望江校区"></img-and-word>
          </div>
      </div>

      <br>

    </div>
  </div>
</template>

<script>
import imgAndWord from "@/components/imgAndWord";
import { ref } from 'vue';
import {Connection} from '../../node_modules/@element-plus/icons-vue';
import back from "@/components/back";
export default {

  // eslint-disable-next-line vue/multi-word-component-names
  name: "home",
  components:{
    imgAndWord,
    Connection,
    back,
  },
  data() {
    return {
      textarea:ref(''),
      note: {
        backgroundImage: "url(" + require("../assets/R-C.png") + ")",
        backgroundRepeat: "no-repeat",
        // backgroundSize: "auto 800px",
        marginTop: "0px",
        width:"100%",
        height:"100%",
        position:"fixed",
        backgroundSize:"100% 100%"
      },
      flag1:1,
    }
  }
}
</script>

<style scoped>
#upput{
  margin-top: 30px;
}
 .title{
   margin-top: 100px;
   color: azure;
   animation: pulse;
   animation-duration: 2s;
 }
 .title2{
   margin-top: 100px;
   color: azure;
 }
 .url{
   color: azure;
 }
 .input{
   margin-left: 20%;
   margin-right: 20%;
 }
 #h1highlight2{
   display: flex;
   justify-content: flex-start;
   margin-top: 0px;
   margin-left: 30px;
 }
 .textButton{
   margin-top: 0px;
   margin-right: 10px;
   ForeColor:white;
   color:white;
   font-size: x-large;
   display: flex;
   justify-content:flex-end;
 }
 .detail{
   display: flex;
   align-items: center;
   justify-content:space-evenly;
   margin-top: 5%;
   margin-left: 20%;
   margin-right: 20%;

 }
</style>