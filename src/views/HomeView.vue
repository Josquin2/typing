<script setup lang="ts">
import { ref } from 'vue'

const allText =
  'To make breakfast, lunch, and dinner daily, these persons must have the required foods and ingredients on hand and ready to go; foods and ingredients are typically purchased from a grocery store, or an establishment that distributes foods, drinks, household products, and other items.'
</script>

<template>
  <div class="main-container">
    <div class="text">
      <div v-for="word in allText.split(' ')" class="one-word">
        <p v-for="letter in word">{{ letter }}</p>
      </div>
    </div>
    <div class="input-area">
      <input type="text" class="border main-input" />
    </div>
  </div>
</template>

<style lang="scss">
.main-container {
  min-height: 80vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  .text {
    margin-top: 100px;
    padding: 0 10vw;
    display: flex;
    height: max-content;
    flex-wrap: wrap;
    .one-word {
      display: flex;
      margin-right: 10px;
      font-size: 20px;
    }
  }

  .input-area {
    margin-top: 80px;
    .main-input {
      padding-left: 16px;
      width: 60vw;
      height: 10vh;
      font-size: 20px;
    }
  }
}
</style>
