<template>
  <div class="home-view">
    <div class="grid-container">
      <div v-for="(item, index) in gridItems" :key="index" class="grid-item">
        <div class="card"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HomeView',
  data() {
    return {
      gridItems: Array(12).fill(null),
    }
  },
}
</script>

<style scoped>
.grid-container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 20px;
  padding: 20px;
  width: calc(100vw - 100px - 200px - 20px);
  /*width: calc(100% - 100px); /* Subtract the width of the right buttons */
}

.grid-item {
  display: flex;
  justify-content: center;
}

.card {
  aspect-ratio: 1;
  flex: 1;
  background-color: #f0f0f0;
  border: 1px solid #ddd;
  border-radius: 10px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  transition: box-shadow 0.3s ease-in-out;
}

.card:hover {
  box-shadow: 0 0 20px rgba(0, 0, 0, 0.3);
}
</style>
