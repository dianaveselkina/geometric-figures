<template>
  <div class="board">
    <h1>Уровень 1</h1>
    <div class="board__wrapper">
      <div class="playing__field">
        <div class="droppable">
          <div class="droppable__circle">
            <DroppableBlock id="circle" imgUrl="/img/circle.png " />
            <input
              class="circle"
              type="checkbox"
              id="circle"
              v-model="checkedNames"
            />
          </div>
          <div class="droppable__triangle">
            <DroppableBlock id="triangle" imgUrl="/img/triangle.png " />
            <input
              class="triangle"
              type="checkbox"
              id="triangle"
              v-model="checkedNames"
            />
          </div>
          <div class="droppable__square">
            <DroppableBlock id="square" imgUrl="/img/square.png " />
            <input
              class="square"
              type="checkbox"
              id="square"
              v-model="checkedNames"
            />
          </div>
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
    return {
      checkedNames: [],
    };
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
.circle,
.square,
.triangle {
  height: 100px;
  width: 100px;
}
.droppable__circle,
.droppable__triangle,
.droppable__square {
  display: flex;
  flex-direction: row;
  align-items: center;
  gap: 100px;
}
</style>
