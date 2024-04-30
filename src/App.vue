<template>
  <div class="app">
    <GameBoard />
  </div>
</template>
<script>
import GameBoard from './components/GameBoard.vue';
export default {
  components: {
    GameBoard,
  },

  data() {
    return {};
  },
  methods: {},
};
</script>
<style>
.app {
  padding: 8px 35px;
  cursor: pointer;
  background-color: #382720;
  border-radius: 6px;
}
</style>
