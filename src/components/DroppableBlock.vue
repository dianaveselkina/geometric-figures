<template>
  <div class="droppable__block">
    <img class="card__img" :src="imgUrl" alt="rose" />
  </div>
</template>
<script setup>
defineProps({
  imgUrl: String,
});
</script>
<style scoped>
.droppable__block {
  display: flex;
  flex-direction: column;
  width: 300px;
  height: 300px;
  padding: 40px;
  cursor: pointer;
  background-color: #ebac9c;
  border-radius: 18px;
  border: solid 1px #948e8d;
}
</style>
