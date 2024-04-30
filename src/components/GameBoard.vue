<template>
  <div class="board">
    <DragBlock imageUrl="/img/square.png " />
    <DragBlock imageUrl="/img/circle.png " />
    <DragBlock imageUrl="/img/triangle.png" />
  </div>
</template>
<script>
import DragBlock from './DragBlock.vue';
export default {
  components: {
    DragBlock,
  },
  data() {
    return {};
  },
  methods: {},
};
</script>

<style>
.board {
  width: 2400px;
  height: 2200px;
  background-color: red;
}
</style>
