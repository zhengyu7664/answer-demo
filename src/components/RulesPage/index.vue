<!--
 * @Author: your name
 * @Date: 2020-07-04 14:00:48
 * @LastEditTime: 2020-07-04 16:27:00
 * @LastEditors: Please set LastEditors
 * @Description: In User Settings Edit
 * @FilePath: \ANSWER\src\components\RulesPage\index.vue
--> 
<template>
  <transition appear name="slide-fade">
    <div class="rules-container">
      <header class="header">
        <!-- <router-link > -->
          <img @click="backHandle" class="close-icon" src="../../assets/icon/close.svg" alt="close">
        <!-- </router-link> -->
        <h1 class="heading">游戏规则</h1>
      </header>
      <div class="content">
        <div class="title">
          <img src="../../assets/icon/tips.svg" alt="tips">
          <h2>玩法介绍</h2>
        </div>
        <p class="details">
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
          这里是内容
        </p>
        <div class="title">
          <img src="../../assets/icon/question.svg" alt="question">
          <h2>常见问题</h2>
        </div>
        <p class="details">
          这里是内容<br>
          这里是内容<br>
          这里是内容<br>
          这里是内容<br>
          这里是内容<br>
          这里是内容<br>
          这里是内容<br>
          这里是内容<br>
          这里是内容<br>
          这里是内容<br>
          这里是内容<br>
          这里是内容<br>
          这里是内容<br>
          这里是内容<br>
          这里是内容<br>
          这里是内容<br>
          这里是内容<br>
          这里是内容<br>
        </p>
      </div>
    </div>
  </transition>
</template>

<script>
export default {
  name: 'RulesPage',
  methods:{
    backHandle(){
      this.$router.replace('/');
    }
  }
};
</script>

<style lang="scss" scoped src="./style.scss"></style>
