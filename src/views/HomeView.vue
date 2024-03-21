<script setup lang="ts">
import { ref } from 'vue'
import CardItem from '../components/CardItem.vue'
import SubmitButton from '../components/SubmitButton.vue'

function colorChange() {
  showColor.value = !showColor.value
}
const showColor = ref(false)
</script>

<template>
  <main>
    <div class="homePage">
      <CardItem>
        <h1 :class="{ colorH1: showColor }">Card</h1>
        <span>Hello</span>
        <SubmitButton :onclick="colorChange">Send inn</SubmitButton>
      </CardItem>
    </div>
  </main>
</template>

<style>
.homePage {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 40px;
}
.colorH1 {
  color: magenta;
}
</style>
