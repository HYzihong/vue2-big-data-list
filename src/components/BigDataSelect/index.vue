<!--
 * @Author: hy
 * @Date: 2021-08-15 20:14:02
 * @LastEditTime: 2021-08-15 21:22:11
 * @LastEditors: Please set LastEditors
 * @Description: In User Settings Edit
 * @FilePath: /vue2-big-data-list/src/components/BigDataSelect/index.vue
-->
<template>
  <div>
    <el-select v-model="value" placeholder="请选择">
      <!-- size 每一行是多高 el-option是多少像素 -->
      <!-- remain 想要一次渲染多少 -->
      <virtual-list :size="35" :remain="7">
        <el-option
          v-for="item in options"
          :key="item.value"
          :label="item.label"
          :value="item.value"
        >
        </el-option>
      </virtual-list>
    </el-select>
    <el-select v-model="value" placeholder="请选择">
      <!-- size 每一行是多高 el-option是多少像素 -->
      <!-- remain 想要一次渲染多少 -->
      <virtual-list :size="35" :remain="7">
        <el-option
          v-for="item in options"
          :key="item.value"
          :label="item.label"
          :value="item.value"
        >
        </el-option>
      </virtual-list>
    </el-select>
    <el-select v-model="value" placeholder="请选择">
      <!-- size 每一行是多高 el-option是多少像素 -->
      <!-- remain 想要一次渲染多少 -->
      <virtual-list :size="35" :remain="7">
        <el-option
          v-for="item in options"
          :key="item.value"
          :label="item.label"
          :value="item.value"
        >
        </el-option>
      </virtual-list>
    </el-select>
    <el-select v-model="value" placeholder="请选择">
      <!-- size 每一行是多高 el-option是多少像素 -->
      <!-- remain 想要一次渲染多少 -->
      <virtual-list :size="35" :remain="7">
        <el-option
          v-for="item in options"
          :key="item.value"
          :label="item.label"
          :value="item.value"
        >
        </el-option>
      </virtual-list>
    </el-select>
    {{ value }}
  </div>
</template>

<script>
import VirtualList from "vue-virtual-scroll-list";
export default {
  components: {
    VirtualList,
  },
  data() {
    return {
      options: [],
      value: 1,
    };
  },
  mounted() {
    let data = [];
    for (let i = 0; i < 500; i++) {
      data.push({
        value: i + 1,
        label: `select${i + 1}项`,
      });
    }
    this.options = data;
  },
};
</script>
