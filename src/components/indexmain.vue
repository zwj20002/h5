<template>
  <div class="main">
    <div class="maintext">
      <h2>产品与服务</h2>
      <p class="htext">根据您对合规性、隔离性等不同要求，为您提供多种选择</p>
    </div>
    <div class="main-body">
      <div v-for="(item, index) in list" :key="index">
        <img :src="`/src/assets/mainsrc/${item.img}`" />
        <p class="p1">{{ item.name }}</p>
        <p class="p2">{{ item.p1 }}</p>
        <p class="p2">{{ item.p2 }}</p>
      </div>
    </div>
    <button class="btn">查看更多</button>
  </div>
</template>

<script setup>
import { ref } from "vue";
const list = [
  {
    img: "1.jpg",
    name: "MES",
    p1: "满足不同类型企业的信息",
    p2: "化部署、改造、升级需求",
  },
  {
    img: "2.jpg",
    name: "DevOps",
    p1: "实现智能、敏捷、精益的",
    p2: "软件自动化流程",
  },
  {
    img: "3.jpg",
    name: "WMS",
    p1: "全过程库存管理",
    p2: "全面提升仓储效率",
  },
  {
    img: "4.jpg",
    name: "硬件研发云",
    p1: "全新的硬件研发平台",
    p2: "助力开发者快速实现产品化",
  },
];
const isrc = "@/src/assets/mainsrc/1.jpg";
</script>

<style scoped>
.main {
  text-align: center;
}
.htext {
  color: #b8b8b8;
}
.maintext{
    margin: 80px 0;
}
.main-body {
  display: flex;
  width: 70%;
  margin: auto;
  justify-content: space-between;
}
.p1 {
  font-size: 20px;
}
.p2 {
  font-size: 13px;
  color: #7e7e7e;
  text-align: left;
}
.btn {
  margin-top: 40px;
  margin-bottom: 50px;
  width: 200px;
  height: 40px;
  border-radius: 10px;
  background-color: #1971b0;
  color: white;
  border-style: none;
  cursor: pointer;
}
</style>
