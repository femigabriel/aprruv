<template>
  <div class="container">
    <div id="header" class="login-header">
      <div class="logo"></div>
    </div>
  </div>

  <div class="login-card">
    <header class="login-header"></header>
    <div id="nav">
      <router-link to="/"
        >Step 1

        <span> Personal Information </span>
      </router-link>
      |
      <router-link to="/about"
        >Step 2

        <span> Business Information </span>
      </router-link>
      <hr />
    </div>
    <router-view />
  </div>
</template>
<script>
export default {
  data() {
    return {
      current: 0,
    };
  },
  methods: {
    previous() {
      this.$emit("previous");
    },
    next() {
      this.$emit("next");
    },
  },
}
</script>
<style>
body {
  font-family: "Raleway", sans-serif;
  font-size: 14px;
  background: url("https://iam.appruve.co/auth/resources/begx7/login/appruve/img/bg-img.png")
    no-repeat center center fixed;
  background-size: cover;
  color: #111;
  background-color: #fff;
  line-height: 1.66666667;
}

.logo {
  background-image: url("https://iam.appruve.co/auth/resources/begx7/login/appruve/img/appruve-logo.svg");
  background-repeat: no-repeat;
  height: 63px;
  width: 300px;
  margin: 0 auto;
}
#app {
 font-family: Avenir, Helvetica, Arial, sans-serif;
  text-decoration: none;
  color: #2c3e50;
}

#nav {
  padding: 30px;
  text-align: center;
}

#nav a {
  font-weight: bold;
  color: #ccc;
  margin-right: -1px;
  padding-bottom: 5px;
  padding-top: 5px;
  line-height: 1.66666667;
  text-decoration: none;
}

#nav a.router-link-exact-active {
  color: #5bc0de;
  text-align: center;
  font-weight: 700;
}
</style>
7
