<template>
  <div class="tictactoe">
    <Board />
  </div>
</template>

<script>
import Board from "./components/board/board.vue";

export default {
  name: 'Tictactoe',
  components: {
    Board
  },
  data: () => ({

  }),
  mounted() {

  }
};
</script>
<style>
* {
  box-sizing: border-box;
}

html,
body,
#root {
  font-family: "Open Sans", sans-serif;
  margin: 0;
  display: flex;
  flex-direction: column;
  /* overflow: hidden; */
  background-color: #E1E2E1 !important;
}
</style>