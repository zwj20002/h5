<template>
  <div class="main">
    <div class="maintext">
      <h2>合作伙伴</h2>
      <p class="htext">携手共赢，推动中国工业互联网快速发展</p>
    </div>
    <img src="../assets/friend.png" class="img"/>
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
  margin-top: 50px;
}
.img{
    width: 100%;
    object-fit: fill;
}
</style>
