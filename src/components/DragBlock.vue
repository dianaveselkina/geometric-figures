<template>
  <div class="drag">
    <img class="card__img" :src="imageUrl" alt="rose" />
  </div>
</template>
<script setup>
defineProps({
  imageUrl: String,
});
</script>
<style>
.drag {
  padding: 8px 35px;
  cursor: pointer;
  background-color: #ea4c14;
  border-radius: 6px;
}
</style>
