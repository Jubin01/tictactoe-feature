<template>
  <div>
    <h4>Current Player: {{ playervar }}</h4>

    <button v-on:click="newGame()">Start new Game</button>

    <h5>Player {{ winner }} won the game!</h5>
    <div class="tictactoe">
        <Square v-for="(value, index) in squares" :value="value" :key="index" @click="makeMove(index)" />
    </div>
  </div>
</template>

<script src="./board.js">
</script>

<style src="./board.css" scoped></style>