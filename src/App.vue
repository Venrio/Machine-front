<template>
  <el-container class="home-container">
    <!--头部区域-->
  <el-header>
    <div>
      <span>机器学习平台</span>
    </div>
  </el-header>
    <!--页面主体区域-->
  <el-container>
    <!--侧边栏-->
    <el-aside width="200px">
      <!--侧边栏菜单区域-->
     <el-menu
      background-color="#545c64"
      text-color="#fff"
      active-text-color="#ffd04b">
      <!--一级菜单-->
      <el-submenu index="1">
        <!--一级菜单模板区域-->
        <template slot="title">
          <!--图标-->
          <i class="el-icon-menu"></i>
           <!--文本-->
          <span>数据集</span>
          </template>
        <!--二级菜单-->
        <el-menu-item-group>
          <el-menu-item index="1-1">
            <i class="el-icon-caret-right"></i>
            <span>选项1</span>
          </el-menu-item>
          <el-menu-item index="1-2">
            <i class="el-icon-caret-right"></i>
            <span>选项2</span>
          </el-menu-item>
          <el-menu-item index="1-3">
            <i class="el-icon-caret-right"></i>
            <span>选项3</span>
            </el-menu-item>
        </el-menu-item-group>
      </el-submenu>
    </el-menu>

<el-menu
      background-color="#545c64"
      text-color="#fff"
      active-text-color="#ffd04b">
      <!--一级菜单-->
      <el-submenu index="1">
        <!--一级菜单模板区域-->
        <template slot="title">
          <!--图标-->
          <i class="el-icon-menu"></i>
           <!--文本-->
          <span>数据集切分器</span>
          </template>
        <!--二级菜单-->
        <el-menu-item-group>
          <el-menu-item index="1-1">
            <i class="el-icon-caret-right"></i>
            <span>选项1</span>
          </el-menu-item>
          <el-menu-item index="1-2">
            <i class="el-icon-caret-right"></i>
            <span>选项2</span>
          </el-menu-item>
          <el-menu-item index="1-3">
            <i class="el-icon-caret-right"></i>
            <span>选项3</span>
            </el-menu-item>
        </el-menu-item-group>
      </el-submenu>
    </el-menu>

<el-menu
      background-color="#545c64"
      text-color="#fff"
      active-text-color="#ffd04b">
      <!--一级菜单-->
      <el-submenu index="1">
        <!--一级菜单模板区域-->
        <template slot="title">
          <!--图标-->
          <i class="el-icon-menu"></i>
           <!--文本-->
          <span>算法</span>
          </template>
        <!--二级菜单-->
        <el-menu-item-group>
          <el-menu-item index="1-1">
            <i class="el-icon-caret-right"></i>
            <span>选项1</span>
          </el-menu-item>
          <el-menu-item index="1-2">
            <i class="el-icon-caret-right"></i>
            <span>选项2</span>
          </el-menu-item>
          <el-menu-item index="1-3">
            <i class="el-icon-caret-right"></i>
            <span>选项3</span>
            </el-menu-item>
        </el-menu-item-group>
      </el-submenu>
    </el-menu>
    </el-aside>
    <!--右侧内容主体-->
    <el-main>
  <el-tabs v-model="activeName" @tab-click="handleClick">
    <el-tab-pane label="代码行" name="first">代码</el-tab-pane>
    <el-tab-pane label="运行结果" name="second">结果</el-tab-pane>
  </el-tabs>

    </el-main>
  </el-container>
</el-container>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
.home-container{
  height:100%;
}
.el-header{
  background-color: #3a3f42;
  display: flex;
  justify-content: space-between;
  padding-left: 50;
  align-items: center;
  color: #fff;
  font-size: 20px;
  > div {
    display: flex;
    align-items:center;
     span{
      margin-left: 15px;
    }
  }
}
.el-aside{
  background-color: #3a3f42;
  height: 100vh;
}
.el-main{
  background-color: #eaedf1;
}
.menu {
  height: 100%;
}
</style>
