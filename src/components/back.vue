<template>
  <div>
  <el-row>
    <el-col :sm="12" :lg="6">
      <el-result style="color: beige"
          icon="success"
          title="Success Tip"
          sub-title="Please follow the instructions"
      >
        <template #extra>
          <el-button type="primary">Back</el-button>
        </template>
      </el-result>
    </el-col>
    <el-col :sm="12" :lg="6">
      <el-result
          icon="warning"
          title="Warning Tip"
          sub-title="Please follow the instructions"
      >
        <template #extra>
          <el-button type="primary">Back</el-button>
        </template>
      </el-result>
    </el-col>
    <el-col :sm="12" :lg="6">
      <el-result
          icon="error"
          title="Error Tip"
          sub-title="Please follow the instructions"
      >
        <template #extra>
          <el-button type="primary">Back</el-button>
        </template>
      </el-result>
    </el-col>
    <el-col :sm="12" :lg="6">
      <el-result icon="info" title="Info Tip">
        <template #sub-title>
          <p>Using slot as subtitle</p>
        </template>
        <template #extra>
          <el-button type="primary">Back</el-button>
        </template>
      </el-result>
    </el-col>
  </el-row>
  </div>
</template>
<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "back",
  data(){
    return{}
  },
}
</script>

<style scoped>
  .main{
    color: azure;
  }
</style>