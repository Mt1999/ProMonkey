<template>
  <div class="header-right">
    <div class="hd-top">
      <span>用户名称：sdceshi ,</span>
        角色：<span>总代</span> 
      <i></i>退出登录<i></i>
      选择语言：
      <div>
        <input type="text" class="input" >
        <ul>
          <li></li>
        </ul>
      </div>
    </div>
    <div class="hd-bot">
      <ul>
        <li>在线用户</li>
        <li>在线用户</li>
        <li>在线用户</li>
        <li>在线用户</li>
        <li>在线用户</li>
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
          label: '黄金糕'
        }, {
          value: '选项2',
          label: '双皮奶'
        }, {
          value: '选项3',
          label: '蚵仔煎'
        }, {
          value: '选项4',
          label: '龙须面'
        }, {
          value: '选项5',
          label: '北京烤鸭'
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
  height: 60px;
  display: flex;
  flex-direction: column;
}
.header-right .hd-top {
  height: 30px;
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
}
.select-input {
  height: 18px;
}
.input-with-select .el-input-group__prepend {
  background-color: #fff;
}


.header-right .hd-bot {
  height: 30px;
}
</style>
