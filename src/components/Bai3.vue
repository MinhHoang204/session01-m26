<template>
  <div class="card">
    <div class="card-image">Image</div>
    <div class="card-title">Title</div>
    <button class="card-button">Add to cart</button>
  </div>
</template>

<script>
export default {
  name: 'Card'
};
</script>

<style scoped>
.card {
  width: 200px;
  border: 1px solid #ddd;
  border-radius: 8px;
  overflow: hidden;
  text-align: center;
  box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.1);
  font-family: Arial, sans-serif;
}

.card-image {
  background-color: #ccc;
  color: black;
  padding: 50px 0;
  font-size: 20px;
  font-weight: bold;
}

.card-title {
  padding: 20px 0;
  font-size: 18px;
  font-weight: bold;
}

.card-button {
  padding: 10px 20px;
  margin-bottom: 20px;
  border: 1px solid #000;
  background-color: white;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.card-button:hover {
  background-color: #f0f0f0;
}
</style>
