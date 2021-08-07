<template>
  <div id="app">
    大家好
    <el-row>
      <el-button>默认按钮</el-button>
      <el-button type="primary">主要按钮</el-button>
      <el-button type="success">成功按钮</el-button>
      <el-button type="info">信息按钮</el-button>
      <el-button type="warning">警告按钮</el-button>
      <el-button type="danger">危险按钮</el-button>
    </el-row>
    <router-view />
  </div>
</template>
// 需要加 lang="ts"
<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  data () {
    return {
      a: 1,
      b: '2'
    }
  },
  methods: {
    test () {
      // this.b.abc()
    }
  }
})
</script>

<style lang="scss" scoped></style>
