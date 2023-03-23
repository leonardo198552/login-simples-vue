<template>
  <div class="login-form">
    <h1>Login</h1>
    <form @submit.prevent="submitForm">
      <div>
        <label for="email">Email:</label>
        <input type="email" id="email" v-model="email" required />
      </div>
      <div>
        <label for="password">Password:</label>
        <input type="password" id="password" v-model="password" required />
      </div>
      <button type="submit">Login</button>
    </form>
  </div>
</template>

<script>
export default {
  data() {
    return {
      email: '',
      password: '',
    };
  },
  methods: {
    submitForm() {
      // Aqui você pode adicionar sua lógica de autenticação, como chamar uma API
      console.log('Email:', this.email);
      console.log('Password:', this.password);
    },
  },
};
</script>

<style scoped>
.login-form {
  width: 300px;
  margin: 0 auto;
}

.login-form h1 {
  text-align: center;
}

.login-form div {
  margin-bottom: 1em;
}

.login-form label {
  display: block;
}
</style>