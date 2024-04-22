<!-- src/App.vue -->

<template>
  <div id="app" class="container">
    <h1 class="title">Login Form</h1>
    <LoginForm />
  </div>
</template>

<script>
import LoginForm from './components/LoginForm.vue';

export default {
  name: 'App',
  components: {
    LoginForm
  }
};
</script>

<style>
.container {
  max-width: 600px;
  margin: 50px auto;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 10px;
  background-color: #f5f5f5;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  background-image: linear-gradient(45deg, #f5f5f5 25%, transparent 25%, transparent 50%, #f5f5f5 50%, #f5f5f5 75%, transparent 75%, transparent);
  background-size: 20px 20px;
}

.title {
  text-align: center;
  color: #333;
  margin-bottom: 20px;
}
</style>
