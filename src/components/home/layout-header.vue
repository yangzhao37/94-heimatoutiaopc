<template>
  <!-- elementUI布局组件 el-row 和 el-col -->
  <el-row align="middle" type="flex" class="layout-header">
      <!-- 等分为两列 为什么是:span="12" 因为span要求的类型是number,加:是让12变为number -->
      <el-col class="left" :span="12">
          <!-- 图标 -->
          <i class="el-icon-s-fold"></i>
          <span>
              江苏传智播客教育科技股份有限公司
          </span>
      </el-col>
      <!-- 右侧列 -->
      <el-col class="right" :span="12">
          <!-- 再次放置一个 row组件 justify属性水平对齐组方式 align属性垂直对齐方式 -->
          <el-row type="flex" justify="end" align="middle">
              <img src="http://b-ssl.duitang.com/uploads/item/201511/21/20151121171107_zMZcy.jpeg" alt="">
          <!-- 下拉菜单 -->
          <el-dropdown trigger="click">
              <!-- 显示的内容 -->
              <span>Y小刀</span>
              <!-- 下拉内容需要做具名插槽dropdown el-dropdown-menu是专门做下拉的组件 -->
              <el-dropdown-menu slot="dropdown">
                  <!-- 下拉选项 el-dropdown-item作为下拉选项的组件 -->
                  <el-dropdown-item>个人信息</el-dropdown-item>
                  <el-dropdown-item>git地址</el-dropdown-item>
                  <el-dropdown-item>退出</el-dropdown-item>
              </el-dropdown-menu>
          </el-dropdown>
          </el-row>
      </el-col>
  </el-row>
</template>

<script>
export default {

}
</script>

<style lang='less' scoped>
   .layout-header {
       height: 60px;
       .left {
           i {
               font-size: 20px;
           }
       }
       .right {
           img {
               width: 40px;
               height: 40px;
               border-radius: 50%;
               margin-right: 4px;
           }
       }
   }
</style>
