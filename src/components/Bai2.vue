<template>
  <div class="box-container">
    <div :class="boxClass" class="box">
      Box
    </div>
    <div class="label">
      {{ color }}
    </div>
  </div>
</template>

<script>
export default {
  name: 'ColorBox',
  props: {
    color: {
      type: String,
      required: true,
      validator(value) {
        return ['red', 'blue', 'green'].includes(value);
      }
    }
  },
  computed: {
    boxClass() {
      return this.color;
    }
  }
};
</script>

<style scoped>
.box-container {
  display: inline-block;
  text-align: center;
  margin: 10px;
}

.box {
  width: 200px;
  height: 200px;
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  font-size: 20px;
  font-weight: bold;
}

.red {
  background-color: red;
}

.blue {
  background-color: blue;
}

.green {
  background-color: green;
}

.label {
  margin-top: 10px;
  font-size: 16px;
  border: 1px solid #ccc;
  padding: 5px;
  display: inline-block;
}
</style>
