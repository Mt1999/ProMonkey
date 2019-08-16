<template>
  <div class="inner">
    <h4>
      <em style="float:right">
        <img src="../assets/refresh.png" alt="刷新">
      </em>
      <span>我的面板</span>
    </h4>
    <el-tree :data="data" :props="defaultProps" @node-click="handleNodeClick"></el-tree>
  </div>
</template>

<script>
export default {
  data() {
    return {
      data: [{
        label: '真人游戏记录',
        children: [{
          label: '百家乐'
        }, {
          label: '龙虎'
        }, {
          label: '牛牛'
        }, {
          label: '单双'
        }, {
          label: '庄闲牛'
        }
        
        ]
      }, {
        label: '真人开奖记录',
        children: [{
          label: '二级 3-1',
          children: [{
            label: '三级 3-1-1'
          }]
        }, {
          label: '二级 3-2',
          children: [{
            label: '三级 3-2-1'
          }]
        }]
      }, {
        label: '对打游戏记录查询',
        children: [{
          label: '百家乐'
        }]
      }],
      defaultProps: {
        children: 'children',
        label: 'label'
      }
    };
  },
  methods: {
    handleNodeClick(data) {
      console.log(data);
    }
  }
};
</script>

<style>
.inner {
  width: 220px;
  height: 100%;
  background-color: #e7f5fe;
  display: flex;
  flex-direction: column;
}
.inner h4 {
  border: 1px solid #069;
  border-width: 0 1px 1px 0;
  margin-top: 0;
  font-size: 14px;
  text-align: left;
  height: 28px;
  line-height: 28px;
  color: #fff;
  width: 219px;
  background-color: #21a9dd;
}
.inner h4 img {
  cursor: pointer;
  width: 14px;
  height: 14px;
  display: block;
  margin-top: 6px;
  margin-right: 10px;
}
.inner h4 span {
  background: url(../assets/arrow.png) no-repeat 5px -1px;
  padding-left: 30px;
}
.el-tree {
  flex: 1;
  background-color: #e7f5fe;
  border-right: 1px solid #069;
}

</style>
