<template>
  <div>
    <!-- 路由容器 -->
    <router-view></router-view>
    <Tabbar></Tabbar>
  </div>
</template>

<script setup>
import Tabbar from './components/Tabbar.vue'

</script>

<style>
*{
  margin: 0;
  padding: 0;
}
ul{
    list-style: none;
}
</style>