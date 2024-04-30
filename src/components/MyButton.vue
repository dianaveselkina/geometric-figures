<template>
  <button class="btn__arrow">
    <img
      class="card__img"
      :src="imgUrl"
      alt="arrow"
      style="width: 80px; height: 80px"
    />
  </button>
</template>
<script setup>
defineProps({
  imgUrl: String,
});
</script>
<style>
.btn__arrow {
  cursor: pointer;
  height: 100px;
  width: 100px;
}
.btn__arrow:hover {
  box-shadow: 0 0 14px 14px rgba(148, 142, 141, 1.6);
}
</style>
