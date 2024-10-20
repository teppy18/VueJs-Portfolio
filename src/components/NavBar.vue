<template>
  <nav class="navbar">
   
    <div class="navbar-logo">
      <h1>My Portfolio</h1>
    </div>

    
    <ul class="navbar-links">
      <li>
        <router-link to="/portfolio/profile">Profile</router-link>
      </li>
      <li>
        <router-link to="/portfolio/showcase">Showcase</router-link>
      </li>
      <li>
        <router-link to="/portfolio/contact">Contact</router-link>
      </li>
      <li>
        <router-link to="/portfolio/creative">Creative</router-link>
      </li>
      <li>
        <router-link to="/login">Logout</router-link> 
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: 'NavBar',
};
</script>

<style scoped>

.navbar {
  background-color: #333;
  padding: 1rem;
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: white;
}

.navbar-logo h1 {
  margin: 0;
  font-size: 24px;
}

.navbar-links {
  list-style: none;
  display: flex;
  gap: 1.5rem;
}

.navbar-links li {
  display: inline;
}

.navbar-links a {
  color: white;
  text-decoration: none;
  font-size: 18px;
  transition: color 0.3s;
}

.navbar-links a:hover {
  color: #f39c12;
}
</style>
