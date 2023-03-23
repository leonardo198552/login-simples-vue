<template>
  <div id="app">
    <login-form></login-form>
  </div>
</template>

<script>
import LoginForm from './components/LoginForm.vue';

export default {
  components: {
    LoginForm,
  },
};
</script>

<style>
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}

#app {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}
</style>