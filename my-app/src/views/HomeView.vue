<template>
  <div class="body">
    <div class="camera-container">
      <div class="image-title">The art of expression and imagination</div>
      <div class="camera-content">
        <img :src="randomImageUrl" alt="Random Image" class="camera-image" />
        <button @click="getRandomImage" class="camera-button">
          <i class="fas fa-camera"></i> Capture 📷
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      randomImageUrl: 'https://source.unsplash.com/500x400/?random',
    };
  },
  methods: {
    getRandomImage() {
      this.randomImageUrl = `https://source.unsplash.com/500x400/?random&t=${Date.now()}`;
    },
  },
};
</script>

<style scoped>
.body {
  background-color: #000;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  margin: 0;
}

.camera-container {
  position: relative;
  text-align: center; 
}

.image-title {
  color: #fff; 
  font-size: 3.5rem; 
  font-family: 'Bagel Fat One', cursive; 
  margin-bottom: 20px; 
}

.camera-content {
  background-color: #222;
  border: 2px solid #fff;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 20px;
}

.camera-image {
  max-width: 100%;
}

.camera-button {
  background-color: #c0c0c0; 
  color: #000;
  border: none;
  padding: 10px 20px;
  border-radius: 5px;
  font-size: 1rem;
  cursor: pointer;
  margin-top: 10px;
  transition: background-color 0.3s ease, transform 0.2s ease, box-shadow 0.3s ease;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: 'Bagel Fat One', cursive; 
  font-size: 1.5rem; 
}

.camera-button i {
  margin-right: 10px;
  font-size: 1.5rem; 
}

.camera-button:hover {
  background-color: #a0a0c0; 
  transform: scale(1.05);
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
}
</style>
