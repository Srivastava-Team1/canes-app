<template>
    <div class="login-container">
      <div class="login-box">
        <img
          src="../assets/canes-logo.png"
          alt="Raising Cane's logo"
          class="canes-logo"
        />
        <div class="login-buttons">
          <button class="guest-btn" @click="handleGuest">Guest</button>
          <button class="login-btn" @click="handleLogin">Login</button>
        </div>
      </div>
    </div>
  </template>
  
  <script setup lang="ts">
  import { ref } from 'vue'
  
  const username = ref('')
  const password = ref('')
  
  function handleGuest() {
    console.log('Guest mode')
  }
  
  function handleLogin() {
    console.log('Login:', username.value, password.value)
  }
  </script>
  
  <style scoped>
  /* Background */
  .login-container {
    width: 110vw;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background: url("../assets/canes-wallpaper.png") center center no-repeat;
    background-size: cover;
    margin: 0;
    padding: 0;
  }
  
  /* White box */
  .login-box {
    width: 550px;
    height: 500px;
    display: flex;
    flex-direction: column;
    align-items: center;
    border: 2px solid black;
    border-radius: 15px;
    background-color: white;
    padding: 30px;
    box-sizing: border-box;
  }
  
  /* logo */
  .canes-logo {
    width: 400px;
    margin-top: -1px;
    margin-bottom: -50px;
  }
  
  /* Buttons at bottom */
  .login-buttons {
    display: flex;
    gap: 60px;
    margin-top: auto;
    margin-bottom: 20px;
  }
  
  /* Buttons boarder with text style*/
  .guest-btn,
  .login-btn {
    font-style: italic;
    font-size: 18px;
    padding: 10px 20px;
    border: 1px solid red;
    border-radius: 5px;
    background-color: yellow;
    color: black;
    font-weight: bold;
    cursor: pointer;
  }
  
  /* Hover effect */
  .guest-btn:hover,
  .login-btn:hover {
    background-color: red;
    color: yellow;
    border-color: yellow;
  }
  </style>