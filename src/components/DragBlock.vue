<template>
  <div class="draggable__block">
    <img class="card__img" :src="imageUrl" alt="rose" />
  </div>
</template>
<script setup>
defineProps({
  imageUrl: String,
});
</script>
<style scoped>
.draggable__block {
  display: flex;
  flex-direction: column;
  width: 300px;
  height: 300px;
  padding: 40px;
  cursor: pointer;
  background-color: #d8d4d3;
  border-radius: 18px;
  border: solid 1px #948e8d;
}
</style>
