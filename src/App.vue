<template>
  <div>
    <el-empty description="描述文字"></el-empty>
    <el-divider></el-divider>
    <el-switch
      v-model="value1"
      active-text="按月付费"
      inactive-text="按年付费">
    </el-switch>
    <el-switch
      style="display: block"
      v-model="value2"
      active-color="#13ce66"
      inactive-color="#ff4949"
      active-text="按月付费"
      inactive-text="按年付费">
    </el-switch>
  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return {
      value1: true,
      value2: true，
      tableData: [{
          date: '2016-05-02',
          name: '王小虎',
          province: '上海',
          city: '普陀区',
          address: '上海市普陀区金沙江路 1518 弄',
          zip: 200333
        }, {
          date: '2016-05-04',
          name: '王小虎',
          province: '上海',
          city: '普陀区',
          address: '上海市普陀区金沙江路 1517 弄',
          zip: 200333
        }, {
          date: '2016-05-01',
          name: '王小虎',
          province: '上海',
          city: '普陀区',
          address: '上海市普陀区金沙江路 1519 弄',
          zip: 200333
        }, {
          date: '2016-05-03',
          name: '王小虎',
          province: '上海',
          city: '普陀区',
          address: '上海市普陀区金沙江路 1516 弄',
          zip: 200333
        }]
    }
  },
  methods: {
    handle() {
      this.$message({
        message: '恭喜你，这是一条成功消息',
        type: 'success'
      });
    }
  }
}
</script>

<style>
.el-header, .el-footer {
    background-color: #B3C0D1;
    color: #333;
    text-align: center;
    line-height: 60px;
  }

  .el-aside {
    background-color: #D3DCE6;
    color: #333;
    text-align: center;
    line-height: 200px;
  }

  .el-main {
    background-color: #E9EEF3;
    color: #333;
    text-align: center;
    line-height: 160px;
  }

  body > .el-container {
    margin-bottom: 40px;
  }

  .el-container:nth-child(5) .el-aside,
  .el-container:nth-child(6) .el-aside {
    line-height: 260px;
  }

  .el-container:nth-child(7) .el-aside {
    line-height: 320px;
  }
</style>
