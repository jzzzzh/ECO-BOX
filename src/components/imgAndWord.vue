<template>
<div class="imgAndWord">
<!--  <img class="myImg" src="{{url}}">-->
  <div v-if="url == 1">
  <el-icon color="white" size="30px"><coffee /></el-icon>
  </div>
  <div v-if="url == 2">
    <el-icon color="white" size="30px"><phone /></el-icon>
  </div>
  <div v-if="url == 3">
    <el-icon color="white" size="30px"><message /></el-icon>
  </div>
  <div v-if="url == 4">
    <el-icon color="white" size="30px"><location /></el-icon>
  </div>
  <h1 class="h3">{{msg}}</h1>
  <p class = "para">{{para}}</p>
</div>
</template>

<script>
import {Coffee,Location,Phone,Message} from "../../node_modules/@element-plus/icons-vue";
export default {
  name: "imgAndWord",
  components:{
    Coffee,
    Location,
    Phone,
    Message,

  },
  props: {
    msg: String,
    url: String,
    para:String,
  }
}
</script>

<style scoped>
  .imgAndWord{
    color: beige;
  }
</style>