<!--
 * @Author: your name
 * @Date: 2021-08-15 19:29:32
 * @LastEditTime: 2021-08-15 20:13:50
 * @LastEditors: Please set LastEditors
 * @Description: In User Settings Edit
 * @FilePath: /vue2-big-data-list/src/App.vue
-->
<template>
  <div id="app">
    <HelloWorld msg="vue2 大数据 展示 性能优化" />
    <component :is="comp" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import BigDataSelect from "./components/BigDataSelect/index";
export default {
  name: "App",
  components: {
    HelloWorld,
    BigDataSelect,
  },
  data() {
    return {
      comp: "BigDataSelect",
    };
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
