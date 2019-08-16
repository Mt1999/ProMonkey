<template>
  <div class="header-right">
    <div class="hd-top">
      <span>用户名称：sdceshi ,</span>
        角色：<span>总代</span> 
      <i></i>退出登录<i></i>
      选择语言：
      <el-select v-model="value" placeholder="请选择" size="mini" >
        <el-option
          v-for="item in options"
          :key="item.value"
          :label="item.label"
          :value="item.value"
        >
        </el-option>
      </el-select>
    </div>
    <div class="hd-bot">
      <ul>
        <li>在线用户</li>
        <li>游戏记录</li>
        <li>游戏报表</li>
        <li>用户管理</li>
        <li>我的面板</li>
        <li>系统日志</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
    data() {
      return {
        options: [{
          value: '选项1',
          label: '简体中文'
        }, {
          value: '选项2',
          label: '繁体中文'
        }, {
          value: '选项3',
          label: '英文'
        }, {
          value: '选项4',
          label: '日文'
        }, {
          value: '选项5',
          label: '韩国'
        }],
        value: ''
      }
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.header-right {
  width: 500px;
  float: right;
  height: 56px;
  display: flex;
  flex-direction: column;
}
.header-right .hd-top {
  height: 28px;
  font-size: 12px;
  color: #fff;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}
.header-right .hd-top i{
  width: 1px;
  height: 12px;
  color: #fff;
  display: inline-block;
  background-color: #fff;
  margin: 5px;
}
.header-right .hd-top input{
  width: 130px;
  height: 14px;
}
.el-select .el-input {
  width: 130px;
  height: 14px;
}
.el-select>.el-input {
  display: block;
  height: 14px;
}
>>> .el-input__inner {
  height: 18px;
}
.input__inner {
  height: 18px;
}
.input-with-select .el-input-group__prepend {
  background-color: #fff;
}
.el-select {
  height: 18px;
}
.el-input--suffix {
  height: 18px;
}
>>> .el-input__inner {
  display: block;
}
>>> .el-input--mini .el-input__icon {
  line-height: 0px;
  position: absolute;
  left: -26px;
}


.header-right .hd-bot {
  height: 28px;
}
.header-right .hd-bot ul{
  height: 28px;
  margin: 0;
  display: flex;
  justify-content: flex-end;
}
.header-right .hd-bot ul li{
  height: 22px;
  margin: 0;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 12px;
  color: #fff;
  border: 1px solid #006699;
  padding: 0 5px;
  margin-left: 5px;
  background-color: #027caf;
}

</style>
