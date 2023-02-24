<template>
  <div class="main">
    <div class="mainbody">
      <div v-for="(item,index) in list" :key="index">
        <p class="thead">{{ item.thead }}</p>
        <div class="ttbody">
            <p class="tbody" v-for="(items,index) in item.tbody" :key="index">{{ items }}</p>
        </div>
      </div>
      <div class="phone">
        <div v-for="phones in phone">
            <p class="tbody">{{ phones.name }}</p>
            <p class="pphone">{{ phones.phone }}</p>
        </div>
      </div>
      <div class="wm">
        <img src="../assets/2wm.png" />
        <p class="tbody">扫描二维码</p>
        <p class="tbody">关注官方微信</p>
      </div>
    </div>
    <div class="footer">
        <p>版权所有 Copyright &copy; 2019 XXXXX. AllRights Reserved. 蜀ICP备XXXXXXXX号-X</p>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
const list = [
  {
    thead: "产品服务",
    tbody: [
      "产品服务1",
      "产品服务2",
      "产品服务3",
      "产品服务4",
      "产品服务5",
      "产品服务6",
    ],
  },
  {
    thead: "典型案例",
    tbody: [
      "典型案例1",
      "典型案例2",
      "典型案例3",
      "典型案例4",
      "典型案例5",
      "典型案例6",
    ],
  },
  {
    thead: "关于我们",
    tbody: ["平台介绍", "平台大事记", "联系我们"],
  },
  {
    thead: "快速入口",
    tbody: ["交易平台", "产品服务", "解决方案", "开发者社区"],
  },
];
const phone = [
    {
        name:'售后热线',
        phone:'028-88888888'
    },
    {
        name:'商务热线',
        phone:'028-88888888'
    },
    {
        name:'邮箱地址',
        phone:'service@changhong.com'
    }
]
</script>

<style scoped>
.main {
  background-color: #272727;
  margin-top: 50px;
}
.mainbody {
  display: flex;
  width: 80%;
  margin: auto;
  justify-content: space-between;
}
.thead{
    color: white;
}
.ttbody{
    margin-top: 30px;
}
.tbody{
    color: #8C8C8C;
}

.pphone{
    color: white;
    font-size: 20px;
}
.wm{
    padding-top: 30px;
    text-align: center;
}
.footer{
    border-top: 1px solid #8C8C8C;
    text-align: center;
    height: 50px;
    color: #8C8C8C;
}
</style>
