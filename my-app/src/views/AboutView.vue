<template>
  <div class="about">
    <div class="about-content">
      <h1 class="about-title">About Us</h1>
      <p class="about-description">
        Welcome to our random image web application. We are a dedicated team of passionate developers and creative designers who have come together to craft this platform, providing you with an enjoyable experience of exploring random images from diverse sources. Our mission is to offer you a delightful and inspiring way to discover the beauty of images and ignite your imagination.
      </p>
    </div>
    <div class="our-team">
      <h2 class="team-title">Meet Our Team</h2>
      <div class="team-members">
        <div class="team-member">
          <img src="/nurulhelda.jpg" alt="Nurul Helda Rangkuti" class="team-member-image" />
          <p class="team-member-name">Nurul Helda Rangkuti</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Bagel+Fat+One&display=swap');

.about {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  background-color: #000;
  padding: 20px;
}

.about-content {
  text-align: center;
  margin-bottom: 30px;
}

.about-title {
  font-family: 'Bagel Fat One', cursive;
  font-size: 2.8rem;
  color: #fff;
  text-transform: uppercase;
}

.about-description {
  font-size: 1.6rem;
  max-width: 800px;
  line-height: 1.6;
  margin: 0 auto;
  color: #fff;
}

.team-title {
  font-family: 'Bagel Fat One', cursive;
  font-size: 2.4rem;
  color: #fff;
  text-transform: uppercase;
  margin-bottom: 20px;
}

.team-members {
  display: flex;
  justify-content: center;
}

.team-member {
  text-align: center;
  margin: 0 20px;
}

.team-member-image {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  margin-bottom: 10px;
}

.team-member-name {
  font-size: 1.4rem;
  color: #FFF;
  font-weight: 600;
}
</style>
