<template>
    <div class="signup-container">
      <div class="signup-form">
        <div class="signup-header">
          <h1>Register</h1>
          <p>Please enter your credentials to sign up!</p>
        </div>
        <div class="form-group">
          <label for="name">Name:</label>
          <input type="text" id="name" />
        </div>
        <div class="form-group">
          <label for="email">Email:</label>
          <input type="email" id="email"/>
        </div>
        <div class="form-group">
          <label for="password">Password:</label>
          <input type="password" id="password" />
        </div>
        <div class="button-container">
          <button>Sign Up</button>
          <RouterLink to="/login" class="login-link">Back to Login</RouterLink>
        </div>
      </div>
    </div>
  </template>
  
  <style scoped>
  .signup-container {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 90vh;
  }
  
  .signup-form {
    width: 450px;
    padding: 50px;
    background-color: #1e1e1e;
    border-radius: 20px;
  }
  
  .signup-header {
    margin-bottom: 20px;
    display: flex;
    flex-direction: column;
    color: #fff;
    font-size: 13px;
    font-family: 'Jost', sans-serif; 
    font-weight: bold;
    align-items: center;
    text-align: center;
    border-bottom: 1px solid #e0e0e026;
  }
  
  .signup-header p {
    color: #fff;
    font-size: 15px;
    font-family: 'Jost', sans-serif; 
    font-weight: normal;
  }
  
  .form-group {
    margin-bottom: 20px;
    color: #fff;
  }
  
  label {
    font-family: 'Jost', sans-serif; 
    font-size: 14px;
    font-weight: bold;
    color: #fff;
  }
  
  input[type="email"],
  input[type="password"],
  input[type="text"] {
    padding: 10px;
    border: 1px solid #e0e0e026;
    border-radius: 4px;
    font-family: 'Jost', sans-serif; 
    font-size: 14px;
    margin-bottom: 10px;
    width: 96%;
    margin-top: 5px;
    background-color: transparent;
    color: #fff;
  }
  
  button {
    padding: 10px 20px;
    background-color: white;
    color: #332D2D;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    font-family: 'Jost', sans-serif; 
    transition: background-color 0.5s ease;
    margin-top: 20px;
    width: 100%;
    font-size: 15px;
    border-radius: 30px;
  }
  
  button:hover {
    background-color: rgb(196, 196, 196);
  }
  
  .button-container {
    text-align: center;
  }
  
  .login-link {
    margin-top: 20px;
    color: #fff;
    /*text-decoration: none;*/
    display: inline-block;
    transition: color 0.5s ease;
    font-family: 'Jost', sans-serif; 
    font-size: 12px;
  }
  
  .login-link:hover {
    color: rgb(196, 196, 196);
  }
  </style>
  