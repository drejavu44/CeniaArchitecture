<script setup></script>

<template>
  <div class="hero-section">
    <h1>Welcome to CeNia</h1>
    <p>
      Lorem Ipsum is simply dummy text of the printing and typesetting industry.
    </p>
    <button class="hero-button">Learn More</button>
  </div>
  <div class="about-us">
    <h1>about us</h1>
  </div>
</template>

<style scoped>
.hero-section {
  background-image: url("../assets/cenia-hero.png");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  height: 500px;
  text-align: center;
  align-items: center;
  color: white;
  font-family: "Jost", sans-serif;
  padding: 40px;
}

p{
    font-style: italic;
}

.hero-button{
    background-color: #1e1e1e;
    color: white;
    font-size: 14px;
    border: none;
    padding: 10px 24px;
    border-radius: 30px;
    transition-duration: 0.4s;
}

.hero-button:hover{
    background-color:rgb(43, 43, 43) ;
}
</style>
