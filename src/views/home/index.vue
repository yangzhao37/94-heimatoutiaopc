<template>
  <!-- 先在最外层放置一个大容器，因为，小容器只能放到大容器里面  -->
  <el-container>
    <el-aside style="width:230px">
      <!-- <h1>左侧导航区域</h1> -->
      <!-- 左侧导航组件 -->
      <layout-aside></layout-aside>
    </el-aside>
    <!-- 右侧 再嵌套一个 el-container -->
    <el-container>
      <!-- 再上下布局 -->
      <el-header>
        <!-- <h1>顶部操作栏</h1> -->
        <!-- 顶部操作栏组件 -->
        <layout-header></layout-header>
      </el-header>
      <!-- 主要区域 el-main默认给加了 20px的内边距-->
      <el-main style="padding: 0">
        <h1>主要区域</h1>
        <!-- 这里应该放置 二级路由容器 -->
        <router-view></router-view>
      </el-main>
    </el-container>
  </el-container>
</template>

<script>
// 将左侧导航组件引用 注册 并使用
// import LayoutAside from '@/components/home/layout-aside'
// import LayoutHeader from '@/components/home/layout-header'
export default {
  // components: {
  //   'layout-aside': LayoutAside,
  //   'layout-header': LayoutHeader
  // }
}
</script>

<style>

</style>
