<!--
 * @Author: your name
 * @Date: 2021-08-11 22:57:37
 * @LastEditTime: 2021-08-12 21:31:40
 * @LastEditors: Please set LastEditors
 * @Description: In User Settings Edit
 * @FilePath: /vue2-big-data-list/src/App.vue
-->
<template>
  <div id="app">
    <HelloWorld msg="vue2 大数据 展示 性能优化" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    HelloWorld,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
