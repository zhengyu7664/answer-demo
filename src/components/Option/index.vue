<!--
 * @Author: your name
 * @Date: 2020-07-03 09:19:32
 * @LastEditTime: 2020-07-04 01:46:00
 * @LastEditors: Please set LastEditors
 * @Description: In User Settings Edit
 * @FilePath: \quiz-game\src\components\Option\index.vue
--> 
<template>
  <transition appear name="slide">
    <li
      :class="{ [optionsInfo.state ? 'right' : 'wrong']: optionsInfo.selected }"
      :style="wrongClass"
    >
      <slot />
      <!-- <span class="rate">{{ optionsInfo.selected ? rate : '' }}</span> -->
    </li>
  </transition>
</template>

<script>
export default {
  name: 'Option',
  props: {
    optionsInfo: Object,
    rate: {
      default: '100%',
      type: String
    }
  },
  computed: {
    wrongClass() {
      return {
        // backgroundSize: this.optionsInfo.selected && !this.optionsInfo.state ? `${this.rate} 100%` : ''
        backgroundSize: this.optionsInfo.selected && !this.optionsInfo.state ? `100% 100%` : ''
      };
    }
  }
};
</script>

<style lang="scss" scoped src="./style.scss"></style>
