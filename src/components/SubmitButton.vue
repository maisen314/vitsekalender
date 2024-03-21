<script setup>
defineProps({
  click: Function
})
</script>

<template>
  <!-- pass onClick from parent -->
  <button type="submit" class="button" :onclick="click">
    <slot>Send inn</slot>
  </button>
</template>

<style>
.button {
  background-color: rgb(14, 79, 79);
  color: white;
  border-radius: 4px;
  padding: 4px;
  &:hover {
    color: black;
    background-color: rgb(155, 255, 255);
  }
}
</style>
