<template>
  <div class="square">
    <button :data-player="value" @click="$emit('click')">{{ value }}</button>
  </div>
</template>

<script>
export default {
  name: "Square",
  props: {
    value: {
      type: String,
      required: true
    }
  }
}
</script>

<style scoped>
.square {
  flex: 1;
  flex-basis: 30%;
  border: 1px solid gray;
}

button {
  width: 100%;
  height: 60px;
}

button[data-player="X"] {
  color: darkgreen;
  background-color: aquamarine;
}

button[data-player="O"] {
  color: lightcoral;
  background-color: blanchedalmond;
}
</style>