<template>
  <footer class="footer">
    <div class="footer-content">
      <p>&copy; 2024 David's Portfolio. All rights reserved.</p>
      <div class="footer-social">
        <a href="https://github.com/teppy18" target="_blank" rel="noopener noreferrer">GitHub</a>
        <a href="https://www.linkedin.com/in/david-anthony-p" target="_blank" rel="noopener noreferrer">LinkedIn</a>
        <a href="https://x.com/daviiidanthony" target="_blank" rel="noopener noreferrer">Twitter</a>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooTer',
};
</script>

<style scoped>
.footer {
  background-color: #333;
  color: white;
  padding: 1rem;
  text-align: center;
  width: 100%;
  margin-top: 20px;
}

.footer-content {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.footer-social {
  margin-top: 0.5rem;
}

.footer-social a {
  color: white;
  margin: 0 1rem;
  text-decoration: none;
  font-size: 16px;
  transition: color 0.3s;
}

.footer-social a:hover {
  color: #f39c12; 
}
</style>
