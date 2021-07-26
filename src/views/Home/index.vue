<template>
  <div class="home">
    <div class="block">
      <span class="demonstration">默认</span>
      <el-date-picker
        v-model="value1"
        type="daterange"
        range-separator="至"
        start-placeholder="开始日期"
        end-placeholder="结束日期"
        value-format="yyyy/MM/dd"
      >
      </el-date-picker>
    </div>
    <p>{{ value1 }}</p>
    <h1>{{baseUrl}}</h1>
    <h1>{{upload}}</h1>
    <p>我是Master111</p>
    <p>我是第二次上传</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      value1: "",
      baseUrl:process.env.VUE_APP_BASE_URL,
      upload:process.env.VUE_APP_UPLOAD,
    };
  },
};
</script>

<style scoped>
</style>