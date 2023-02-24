<template>
  <div class="main">
    <div class="left">
      <img src="../assets/logo.png" />
      <p
        v-for="(item, index) in list"
        :key="index"
        :class="defaultindex == index ? 'active-text' : 'head-text'"
        @click="changeindex(index)"
      >
        {{ item }}
      </p>
    </div>

    <div class="right">
        <img src="../assets/搜索.png" class="icon"/>
      <p class="head-text">控制中心</p>
      <p class="head-text">登录</p>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

const defaultindex = ref(0);
const list = [
  "首页",
  "交易平台",
  "产品",
  "工业APP",
  "解决方案",
  "行业专家",
  "开发者平台",
  "新闻资讯",
  "关于我们",
];

const changeindex = (index) => {
  defaultindex.value = index;
};
</script>

<style scoped>
.main {
  height: 60px;
  background-color: #020202;
  display: flex;
  justify-content: space-between;
  padding: 0 20px;
}
.left{
    display: flex;
    align-items: center;
}
.head-text {
  color: white;
  margin: 0 10px;
  font-size: 13px;
}
.active-text {
  color: #47618f;
  margin: 0 10px;
  font-size: 13px;
}
.right {
  display: flex;
  align-items: center;
}
.icon{
    height: 18px;
    width: 18px;
    margin-right: 5px;
}
</style>
