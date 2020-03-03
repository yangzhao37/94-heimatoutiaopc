<template>
  <!-- 二级路由的默认组件 -->
  <div class="second_home">
    <!-- 幻灯片 -->
    <el-carousel height="200px" direction="vertical" :autoplay="false">
      <el-carousel-item v-for="item in 3" :key="item">
        <h3 class="medium">{{ item }}</h3>
      </el-carousel-item>
    </el-carousel>
  </div>
</template>

<script>
export default {
  data () {
    return {
      list: [

      ]
    }
  }
}
</script>

<style>
.second_home {
  /* calc 计算的意思 在css上计算数值 用法 calc ( 四则运算 ) 变量 和运算符 之间一定要有空格*/
  height: calc(100vh - 60px);
  background-size: cover;
  background-image: url(https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=1694681277,1453280371&fm=26&gp=0.jpg);
}
</style>
