<!--
 * @Author: liuzheng 8330460+wx_3078dad3bd@user.noreply.gitee.com
 * @Date: 2023-09-12 17:11:49
 * @LastEditors: liuzheng 8330460+wx_3078dad3bd@user.noreply.gitee.com
 * @LastEditTime: 2023-09-12 22:05:33
 * @FilePath: \vite-project\src\views\Home\index.vue
 * @Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
-->
<template>
  <Header></Header>
  <div class="flex">
    <Navigation></Navigation>
    <div class="">
      <router-view></router-view>
    </div>
  </div>
</template>
<style scoped>
.active {
  font-weight: bold;

  text-decoration: underline;
  text-decoration-color: red;
  text-underline-offset: 0.5em;
}
</style>
<script setup>
import Header from "./components/Header.vue";
import Navigation from "./components/Navigation.vue";
import PersonalityRecommendation from "../Home/Find/PersonalityRecommendation.vue";
import { reactive } from "vue";
import { useRouter } from "vue-router";

const curNode = reactive({ title: "" });
</script>