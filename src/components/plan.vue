<template>
  <div class="main">
    <div class="maintext">
      <h2>解决方案</h2>
      <p class="htext">基于工业互联网平台的行业解决方案</p>
    </div>
    <div>
      <div class="maindiv">
        <div class="mainimg">
          <img src="../assets/plan/1.png" alt="" class="imgs" />
          <img src="../assets/plan/2.png" alt="" class="imgs" />
          <img src="../assets/plan/3.png" alt="" class="imgs" />
          <img src="../assets/plan/4.png" alt="" class="imgs" />
          <img src="../assets/plan/5.png" alt="" class="imgs" />
        </div>
        <button class="btn">查看更多</button>
      </div>
      <img src="../assets/bkimg.png" class="img" />
      <img src="../assets/doc.png"/>
      <button class="btn">查看更多</button>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
</script>

<style scoped>
.main {
  text-align: center;
}
.htext {
  color: #b8b8b8;
}
.maintext {
  margin: 80px 0;
}
.maindiv {
  position: absolute;
  overflow: hidden;
  width: 85%;
  left: 7%;
}
.mainimg {
  display: flex;
  justify-content: space-around;
  overflow: hidden;
}
.img {
  margin-top: 150px;
  width: 100%;
  object-fit: fill;
}
.imgs {
  width: 240px;
  object-fit: fill;
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
