<template>
  <div id="app">
    <el-container>
      <el-header class="elHeader">
        <!-- 头部 -->
        <Sq-Header></Sq-Header>
        
      </el-header>
      <el-container>
        <!-- 侧边栏 -->
        <sq-sidebar></Sq-Sidebar>

        <el-main>
          <!-- 内容 -->
          <Sq-Main></Sq-Main>
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
/* 重置样式 */
html, body, div, span, applet, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, big, cite, code,
del, dfn, em, img, ins, kbd, q, s, samp,
small, strike, strong, sub, sup, tt, var,
b, u, i, center,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, embed,
figure, figcaption, footer, header, hgroup,
menu, nav, output, ruby, section, summary,
time, mark, audio, video {
  margin: 0;
  padding: 0;
  border: 0;
  font-size: 100%;
  font: inherit;
  vertical-align: baseline;
}
 /* HTML5 display-role reset for older browsers */
article, aside, details, figcaption, figure,
footer, header, hgroup, menu, nav, section {
  display: block;
}
body {
  line-height: 1;
}
ol, ul, li {
  list-style: none;
}
blockquote, q {
  quotes: none;
}
blockquote:before, 
blockquote:after,
q:before,
q:after {
  content: '';
  content: none;
}
table {
  border-collapse: collapse;
  border-spacing: 0;
}
body,
html {
  width: 100%;
  height: 100%;
}
main {
  width: 100%;
  flex: 1;
  overflow-x: hidden;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */
  height: 100%;
}
.el-container {
  height: 100%;
}
.el-header, .el-footer {
  background-color: #1ea4d7;
  color: #333;
  text-align: center;
  line-height: 56px;
  border-bottom: 5px solid #069;
}
.elHeader {
  height: 56px;
  border-top: 1px solid #006599;
}

.el-main {
  background-color: #E9EEF3;
  color: #333;
  text-align: center;
  line-height: 160px;
  padding: 0;
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
.el-aside {
  background-color: #D3DCE6;
  color: #333;
  text-align: center;
  line-height: 200px;
  width: 220px;
}



</style>
