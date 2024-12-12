<template>
  <div class="layout">
    <nav class="left-navbar">
      <ul>
        <li><RouterLink to="/">Home</RouterLink></li>
        <li><RouterLink to="/about">About</RouterLink></li>
      </ul>
    </nav>
    <div class="right-buttons">
      <button class="round-button">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 24 24"
          fill="none"
          stroke="currentColor"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
          class="icon"
        >
          <path
            d="M21 12c0 6.075-4.925 11-11 11S3 18.075 3 12 7.925 3 12 3s9 4.925 9 11Z"
          ></path>
        </svg>
      </button>
      <button class="round-button">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 24 24"
          fill="none"
          stroke="currentColor"
          stroke-width="2"
          stroke-linecap="round"
          stroke-linejoin="round"
          class="icon"
        >
          <path
            d="M21 12c0 6.075-4.925 11-11 11S3 18.075 3 12 7.925 3 12 3s9 4.925 9 11Z"
          ></path>
        </svg>
      </button>
    </div>
    <div class="main-content">
      <RouterView />
    </div>
  </div>
</template>

<script>
export default {
  name: 'Layout',
}
</script>

<style scoped>
.layout {
  display: flex;
  flex-direction: row;
  height: 100vh;
}

.left-navbar {
  position: fixed;
  top: 0;
  left: 0;
  width: 200px;
  height: 100vh;
  background-color: #f0f0f0;
  padding: 20px;
}

.left-navbar ul {
  list-style: none;
  padding: 0;
  margin: 0;
}

.left-navbar li {
  margin-bottom: 10px;
}

.right-buttons {
  position: fixed;
  top: 50%;
  transform: translateY(-50%);
  right: 20px;
}

.main-content {
  margin-left: 200px;
  padding: 20px;
}

.round-button {
  width: 60px;
  height: 60px;
  background-color: #fff;
  border: 2px solid #000;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  cursor: pointer;
  transition:
    background-color 0.1s ease-in-out,
    transform 0.1s ease-in-out;
}

.right-buttons button:not(:first-child) {
  margin-top: 20px;
}

.right-buttons button:hover {
  background-color: #f0f0f0;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.right-buttons button:active {
  transform: scale(0.9);
  background-color: #e0e0e0;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
}

.icon {
  width: 30px;
  height: 30px;
}
</style>
