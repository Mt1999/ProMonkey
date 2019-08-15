<template>
  <div id="app">
    <el-container>
      <el-header>
        <!-- 头部 -->
        <Sq-Header></Sq-Header>
        
      </el-header>
      <el-container>
        <!-- 侧边栏 -->
        <sq-sidebar></Sq-Sidebar>

        <el-main>
          Main
          <!-- 内容 -->

        </el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script>
import SqHeader from './components/SqHeader.vue'
import SqSidebar from './components/SqSidebar.vue'
import SqMain from './components/SqMain.vue'

export default {
  name: 'app',
  components: {
    SqHeader,
    SqSidebar,
    SqMain
  },
  data() {
    return {
      activeName: 'first'
    };
  },
  methods: {
    handleClick(tab,event) {
      console.log(tab,event)
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


.tag {
  float: right;
}
.sidebar {
  width: 200px;
  height: 16px;
}
.sidebar span {
  font-size: 12px;
}
</style>
