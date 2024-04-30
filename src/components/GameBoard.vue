<template>
  <div class="board">
    <h1>Уровень 1</h1>
    <div class="board__wrapper">
      <div class="playing__field">
        <div class="droppable">
          <DroppableBlock imgUrl="/img/circle.png " />
          <DroppableBlock imgUrl="/img/triangle.png " />
          <DroppableBlock imgUrl="/img/square.png " />
        </div>
        <div class="draggable">
          <DragBlock imageUrl="/img/square.png " />
          <DragBlock imageUrl="/img/circle.png " />
          <DragBlock imageUrl="/img/triangle.png " />
        </div>
      </div>
      <div class="btn">
        <MyButton imgUrl="/img/arrow-left.png " />
        <MyButton imgUrl="/img/arrow-right.png " />
      </div>
    </div>
  </div>
</template>
<script>
import DragBlock from './DragBlock.vue';
import DroppableBlock from './DroppableBlock.vue';
import MyButton from './MyButton.vue';
export default {
  components: {
    DragBlock,
    DroppableBlock,
    MyButton,
  },
  data() {
    return {};
  },
  methods: {},
};
</script>

<style scoped>
h1 {
  text-align: center;
  font-size: 60px;
}
.droppable {
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  height: 1800px;
}
.draggable {
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  height: 1800px;
}
.board {
  margin: 0 auto;
  padding: 50px 0;
  width: 2400px;
  height: 2400px;
  background-color: rgb(211, 211, 211);
}
.board__wrapper {
  border-radius: 18px;
  border: solid 1px #636363;
  margin: 30px;
  display: flex;
  flex-direction: column;
  justify-content: space-around;
}
.playing__field {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
}
.btn {
  padding: 100px 400px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
</style>
