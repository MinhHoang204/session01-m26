<template>
  <div class="calculation-container">
    <h2>Simple Calculator</h2>
    
    <div class="input-container">
      <label>Number 1:</label>
      <input v-model.number="number1" type="number" />

      <label>Number 2:</label>
      <input v-model.number="number2" type="number" />
    </div>

    <div class="result-container">
      <p>Addition ({{ number1 }} + {{ number2 }}): {{ addResult }}</p>
      <p>Subtraction ({{ number1 }} - {{ number2 }}): {{ subtractResult }}</p>
      <p>Multiplication ({{ number1 }} * {{ number2 }}): {{ multiplyResult }}</p>
      <p>Division ({{ number1 }} / {{ number2 }}): {{ divideResult }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Calculation',
  data() {
    return {
      number1: 0,
      number2: 0
    };
  },
  computed: {
    addResult() {
      return this.add(this.number1, this.number2);
    },
    subtractResult() {
      return this.subtract(this.number1, this.number2);
    },
    multiplyResult() {
      return this.multiply(this.number1, this.number2);
    },
    divideResult() {
      return this.number2 !== 0 ? this.divide(this.number1, this.number2) : 'Cannot divide by zero';
    }
  },
  methods: {
    add(a, b) {
      return a + b;
    },
    subtract(a, b) {
      return a - b;
    },
    multiply(a, b) {
      return a * b;
    },
    divide(a, b) {
      return a / b;
    }
  }
};
</script>

<style scoped>
.calculation-container {
  max-width: 400px;
  margin: auto;
  text-align: center;
  font-family: Arial, sans-serif;
}

.input-container {
  margin-bottom: 20px;
}

input {
  margin-left: 10px;
  padding: 5px;
  font-size: 16px;
  width: 80px;
}

.result-container {
  margin-top: 20px;
}

p {
  font-size: 18px;
}
</style>
