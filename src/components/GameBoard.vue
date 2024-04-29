<template>
  <div class="board">
    <DragBlock />
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
  width: 1200px;
  height: 1200px;
  background-color: red;
}
</style>
