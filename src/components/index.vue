<template>
  <div class="mains">
    <heade />
    <img src="../assets/inimg.png" class="imgs"/>
    <indexmain />
    <img src="../assets/bkimg.png" class="img" />
    <plan />
    <footers />
    <footertext />
  </div>
</template>

<script setup>
import footers from "./footer.vue";
import  heade  from "./headers.vue";
import indexmain from "./indexmain.vue";
import plan from "./plan.vue";
import footertext from './footertext.vue';
</script>

<style scoped>
.mains{
    background-color: #F4F4F4;
    overflow: hidden;
}
.imgs{
    width: 100%;
    background-color: #F4F4F4;
    object-fit: fill;
}
</style>
