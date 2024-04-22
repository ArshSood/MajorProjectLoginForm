<!-- src/components/LoginForm.vue -->

<template>
  <form @submit.prevent="login" class="login-form">
    <div class="form-group">
      <label for="email">Email:</label>
      <input type="email" id="email" v-model="email" required>
    </div>
    <div class="form-group">
      <label for="password">Password:</label>
      <input type="password" id="password" v-model="password" required>
    </div>
    <button type="submit" class="btn-primary">Login</button>
  </form>
</template>

<script>
export default {
  data() {
    return {
      email: '',
      password: ''
    };
  },
  methods: {
    login() {
      // Implement your login logic here
      console.log('Email:', this.email);
      console.log('Password:', this.password);
      // Example: You can send a request to your backend for authentication
    }
  }
};
</script>

<style scoped>
.login-form {
  max-width: 275px;
  margin: 0 auto;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 5px;
  background-color: #f9f9f9;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  background-image: linear-gradient(45deg, #f5f5f5 25%, transparent 25%, transparent 50%, #f5f5f5 50%, #f5f5f5 75%, transparent 75%, transparent);
  background-size: 20px 20px;
}

.form-group {
  margin-bottom: 15px;
}

label {
  font-weight: bold;
  color: #333;
}

input[type="email"],
input[type="password"],
button {
  width: 90%;
  padding: 10px;
  margin-top: 5px;
  border: 2px solid #ccc;
  border-radius: 3px;
}

button {
  background-color: #007bff;
  color: #fff;
  cursor: pointer;
}

button:hover {
  background-color: #0056b3;
}

.btn-primary {
  margin-top: 20px;
}
</style>
