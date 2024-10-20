<template>
    <div class="creative-page">
      <h2>My Hobbies</h2>
      <ul class="hobby-list">
        <li v-for="(hobby, index) in hobbies" :key="index" class="hobby-item">
          
          <div class="hobby-info">
            <h3>{{ hobby.name }}</h3>
            <p>{{ hobby.description }}</p>
          </div>
        </li>
      </ul>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        hobbies: [
          {
            name: 'Playing FPS Games',
            description: 'Games like CSGO and Valorant',
            
          },
          {
            name: 'Watching Movies and Anime',
            description: 'Streaming on Netflix and exploring new films',
            
          },
          {
            name: 'Exploring and Trying New Things',
            description: 'Learning new things and working on side projects',
            
          }
        ]
      };
    }
  };
  </script>
  
  <style scoped>
  .creative-page {
    max-width: 800px;
    margin: 0 auto;
    padding: 20px;
    background-color: #f8f9fa;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  }
  
  h2 {
    text-align: center;
    margin-bottom: 20px;
    color: #333;
  }
  
  .hobby-list {
    list-style: none;
    padding: 0;
  }
  
  .hobby-item {
    display: flex;
    align-items: center;
    background-color: #fff;
    border: 1px solid #ddd;
    border-radius: 8px;
    margin-bottom: 15px;
    padding: 10px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }
  
  .hobby-icon {
    width: 50px;
    height: 50px;
    margin-right: 15px;
    border-radius: 5px;
    object-fit: cover;
  }
  
  .hobby-info {
    flex: 1;
  }
  
  .hobby-info h3 {
    margin: 0;
    color: #555;
  }
  
  .hobby-info p {
    margin: 5px 0 0;
    color: #777;
  }
  </style>
  