<template>
    <div class="portfolio-showcase">
      <div class="project-card" v-for="project in projects" :key="project.id">
        <img :src="project.image" alt="Project Image" />
        <h3>{{ project.title }}</h3>
        <p>{{ project.description }}</p>
        
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        projects: [
          {
            id: 1,
            title: "ExpressRailway: Online QR code ticketing System For PNR",
            description: "This project intends to make ticketing more effective and convenient for passengers by allowing them to purchase and receive tickets digitally via a website.",
            image: require('@/assets/pnr.png'),
            
          },
          {
            id: 2,
            title: "Cultivation System with AI-Driven Prediction for a Precise Production of Spirulina spp. ",
            description: "The Study on AI-Driven Predictive and Automated System for Spirulina Cultivation represents an improvement in Spirulina production.",
            image: require('@/assets/spp.png'),
            
          }
        ]
      };
    }
  };
  </script>
  
  <style>
  .project-card {
    border: 1px solid #ccc;
    padding: 16px;
    border-radius: 8px;
    transition: transform 0.3s;
  }
  .project-card:hover {
    transform: scale(1.05);
  }
  </style>
  