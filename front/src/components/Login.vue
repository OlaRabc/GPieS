<template>
  <div class="loginPage">
    <form @submit.prevent="login">
      <label> Username: </label>
      <input v-model="username" type="text" />
      <label> Password: </label>
      <input id="password" v-model="password" type="password" />

      <button type="submit">Log in</button>
    </form>
  </div>
</template>

<style scoped>
.loginPage {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  font-family: "Nunito", sans-serif;
  margin: 128px 0px;
}
form {
  border: 1px solid black;
  border-radius: 5px;
  padding: 128px 16px;
  width: 50%;

  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;

  box-shadow: 12px 12px 2px 1px #b3bcc7;
}
input {
  margin-bottom: 16px;
}
button {
  background: #e1ecfa;
  color: #495f7a;
  border: none;
  border-radius: 5px;
  padding: 8px 32px;
  transition: color 0.75s, background-color 0.75s;
  font-weight: 700;
  font-size: 1.2rem;
}
button:hover {
  background: #96c2fb;
  color: #495f7a;
  transition: color 0.75s, background-color 0.75s;
}
</style>
<script>
export default {
  data() {
    return {
      username: "",
      password: "",
    };
  },
  methods: {
    login() {
      // Make an HTTP request to authenticate the user's credentials
      // and set the login state
    },
  },
};
</script>
