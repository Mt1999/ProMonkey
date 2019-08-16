<template>
  <div class="admin_right">
    <div class="directive">
      <div class="pointer">

      </div>
      <span>
        <a href="#" target="right" rel="noopener noreferrer">
          <img src="../assets/refresh.png" title="短信息">
        </a>
        <a href="#" title="后台管理地图">
          <img src="../assets/refresh.png" title="后台管理地图">
        </a>
        <a href="#" title="添加常用操作">
          <img src="../assets/refresh.png" title="添加常用操作">
        </a>
        <a href="#" >
          <img src="../assets/refresh.png" title="菜单搜索">
        </a>
        <a href="#" >
          <img src="../assets/refresh.png" title="扫描木马">
        </a>
        <a href="#" >
          <img src="../assets/refresh.png" title="备忘录">
        </a>
        <a href="#" >
          <img src="../assets/refresh.png" title="使用帮助,按F2也可以打开帮助">
        </a>
      </span>
    </div>
    <div class="scroll-wrapper">
      <div class="table_info">
        <h4>快捷操作</h4>
        <div class="input_button">
          <el-row>
            <el-button size="mini" type="primary" disabled class="j">返回至上一页</el-button>
            <el-button size="mini" type="primary" disabled>前进至下一页</el-button>
            <el-button size="mini" type="primary" disabled>刷新本页</el-button>
            <el-button size="mini" type="primary" disabled>全屏刷新</el-button>
            <el-button size="mini" type="primary" disabled>打印</el-button>
          </el-row>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

</script>

<style>
.admin_right {
  height: 100%;
}
.admin_right .directive {
  height: 28px;
  border-bottom: 1px solid #006699;
}
.admin_right .directive .pointer {
  width: 12px;
  height: 12px;
  background-color: #2b80aa;
  border: 1px solid #006699;
  margin: 7px;
  float: left;
}
.admin_right .directive span {
  float: right;
  height: 28px;
  width: 200px;
  display: flex;
  justify-content: space-around;
  align-items:  center;
}
.admin_right .directive span a {
 width: 18px;
 height: 18px;
}
.admin_right .directive span a img {
 width: 18px;
 height: 18px;
 display: block;
}
.admin_right .scroll-wrapper {
  height: 100%;
}
.admin_right .scroll-wrapper .table_info {
  width: 98%;
  height: 210px;
  margin: 7px auto;
  background: #D5EDFD;
  border: 1px solid #99d3fb;
}
.admin_right .scroll-wrapper .table_info h4 {
  border-bottom-width: 0;
  font-weight: bold;
  color: #077ac7;
  background: url() repeat-x 0 0;
  height: 27px;
  line-height: 27px;
  /* margin: 6px auto 0; */
  font-size: 12px;
  font-family: "宋体";
  border-bottom: 1px solid #99d3fb;        
}
.admin_right .scroll-wrapper .table_info .input_button {
  height: 30px;
  border-bottom: 1px solid #99d3fb;      
  display: flex;
  align-items: center;  
}
.el-row {
  height: 20px;
  display: flex;
  
}
.el-button--mini {
  padding: 3px 3px;
}
.j {
  margin-left: 10px;
}
</style>
