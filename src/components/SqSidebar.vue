<template>
  <el-aside width="200px">
    <el-row class="tac">
        <el-col :span="12" class="sidebar">
            <el-menu
            default-active="2"
            class="el-menu-vertical-demo"
            @open="handleOpen"
            @close="handleClose"
            background-color="#e7f5fe"
            text-color="#000000"
            active-text-color="#ffd04b">
            <el-submenu index="1">
                <template slot="title">
                <i class="el-icon-location"></i>
                <span>真人游戏记录</span>
                </template>
                <el-menu-item-group>
                <!-- <template slot="title">分组一</template> -->
                <el-menu-item index="1-1">百家乐</el-menu-item>
                <el-menu-item index="1-2">龙虎</el-menu-item>
                <el-menu-item index="1-3">庄闲牛</el-menu-item>
                <el-menu-item index="1-4">牛牛</el-menu-item>
                </el-menu-item-group>
            </el-submenu>
            </el-menu>
        </el-col>
    </el-row>
    </el-aside>
</template>

<script>
export default {
    methods: {
      handleOpen(key, keyPath) {
        console.log(key, keyPath);
      },
      handleClose(key, keyPath) {
        console.log(key, keyPath);
      }
    }
  }
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
 .el-header, .el-footer {
    background-color: #1ea4d7;
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
