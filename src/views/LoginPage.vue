<template>
    <div class="login-container">
      <h2>Login</h2>
      <form @submit.prevent="login" class="login-form">
        <input 
          v-model="username" 
          placeholder="Username" 
          class="input-field" 
        />
        <input 
          v-model="password" 
          type="password" 
          placeholder="Password" 
          class="input-field" 
        />
        <button type="submit" class="login-button">Login</button>
      </form>
      <p v-if="error" class="error-message">{{ error }}</p>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        username: '',
        password: '',
        error: ''
      };
    },
    methods: {
      login() {
        if (this.username === 'David' && this.password === 'CPE') {
          this.$router.push('/portfolio/profile');
        } else {
          this.error = 'Invalid login credentials';
        }
      }
    }
  };
  </script>
  
  <style scoped>
  .login-container {
    max-width: 300px;
    margin: 0 auto;
    padding: 2rem;
    background-color: #5d5d5d;
    border: 1px solid #000000;
    border-radius: 8px;
    box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    text-align: center;
  }
  
  h2 {
    margin-bottom: 1.5rem;
    color: #ffffff;
    font-size: 1.5rem;
  }
  
  .login-form {
    display: flex;
    flex-direction: column;
  }
  
  .input-field {
    margin-bottom: 1rem;
    padding: 0.5rem;
    border: 1px solid #ddd;
    border-radius: 4px;
    font-size: 1rem;
  }
  
  .login-button {
    background-color: #000000;
    color: white;
    border: none;
    padding: 0.75rem;
    border-radius: 4px;
    font-size: 1rem;
    cursor: pointer;
    transition: background-color 0.3s;
  }
  
  .login-button:hover {
    background-color: #dddddd;
  }
  
  .error-message {
    color: #e74c3c;
    margin-top: 1rem;
    font-size: 0.9rem;
  }
  </style>
  