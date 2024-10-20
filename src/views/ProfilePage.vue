<template>
    <div class="profile-page">
      <div class="profile-image">
        <img :src="photo" alt="Profile Picture" />
      </div>
      <div class="profile-details">
        <h2>{{ name }}</h2>
        <p>{{ bio }}</p>
        <div class="social-links">
          <a :href="social.facebook" target="_blank" rel="noopener">
            <i class="fab fa-facebook"></i>
          </a>
          <a :href="social.linkedin" target="_blank" rel="noopener">
            <i class="fab fa-linkedin"></i>
          </a>
          <a :href="social.github" target="_blank" rel="noopener">
            <i class="fab fa-github"></i>
          </a>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        name: "David Anthony P. Libao",
        bio: "A graduate of Computer Engineering at Technological Institute of the Philippines. Hard-working, result-driven, dedicated and detail oriented with a passion for technology leveraging my academic background to help a company or organization gain competitive advantage. Eager to pursue a career path that values innovation, problem solving, and collaboration. ",
        photo: require('@/assets/pic.jpeg'),
        social: {
          facebook: "https://www.facebook.com/share/y9jV4eu7kFDcCPkb/?mibextid=LQQJ4d",
          linkedin: "https://linkedin.com/in/david-anthony-p",
          github: "https://github.com/teppy18"
        }
      };
    }
  };
  </script>
  
  <style scoped>
  .profile-page {
    text-align: center;
    padding: 20px;
    margin-bottom: 60px; /* Adds space at the bottom to avoid overlap with the footer */
  }
  
  .profile-image img {
    width: 200px;
    height: 200px;
    border-radius: 15%;
    object-fit: cover;
    margin-bottom: 15px;
  }
  
  .profile-details h2 {
    margin: 20px 0;
    font-size: 24px;
    color: #333;
  }
  
  .profile-details p {
    font-size: 16px;
    color: #555;
    margin-bottom: 20px;
    max-width: 800px;
    margin: 0 auto;
  }
  
  .social-links a {
    display: inline-block;
    margin: 0 10px;
    color: #0099f9;
    font-size: 24px;
    transition: color 0.3s;
  }
  
  .social-links a:hover {
    color: #012254;
  }
  </style>
  