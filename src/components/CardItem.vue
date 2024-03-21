<template>
  <div class="cardItem">
    <slot>placeholder</slot>
  </div>
</template>

<style>
.cardItem {
  display: flex;
  flex-direction: column;
  border: 2px solid black;
  border-radius: 30px;
  width: 50%;
  height: 30vh;
  align-items: center;
  justify-content: center;
}
</style>
