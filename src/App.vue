<template>
  <div id="app">
    <!-- 头部板块 -->
    <app-header></app-header>
    <div class="container-fluid">
      <div class="row">
        <!-- 侧边栏 -->
        <app-sidebar></app-sidebar>

        <!-- 列表 -->
        <router-view></router-view>
      </div>
    </div>
  </div>
</template>

<script>
// 导入公共板块
import AppHeader from './conponents/AppHeader.vue';
import AppSidebar from './conponents/AppSidebar.vue';
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  components:{
    AppHeader,
    AppSidebar
  }
}
</script>

<style>

</style>
