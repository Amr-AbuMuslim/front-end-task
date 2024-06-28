<template>
  <header class="header">
    <div class="container">
      <div class="logo"><img src="../assets/weblogo.png" alt="" /></div>
      <nav class="nav">
        <router-link to="/">Home</router-link>
        <router-link to="/about">About</router-link>
        <router-link to="/blog">Blog</router-link>
        <router-link to="/cart">Cart</router-link>
        <router-link to="/login" class="login">Login</router-link>
        <router-link to="/signup" class="signup">Sign Up</router-link>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
};
</script>

<style lang="scss" >
.header {
  position: sticky;
  background: transparent;
  transition: 1.5s ease;
  height: 80px;
  background-color: #00000040;
}

.header .container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 0px 30px;
}

.logo {
  font-size: 24px;
  font-weight: bold;
  color: #fff;
  width: 150px;
  img {
    max-width: 100%;
  }
}

.nav {
  display: flex;
  align-items: center;
  gap: 20px;
  padding: 20px 0px;
}

.nav a {
  color: #fff;
  text-decoration: none;
  font-weight: 400;
  margin-left: 35px;
}
.nav a.login {
  border: 1px solid var(--main-color);
  border-radius: 16px;
  padding: 5px 10px;
}

.nav a.signup {
  background-color: var(--main-color);
  padding: 5px 10px;
  border-radius: 16px;
  font-weight: 500;
}

.nav a:hover {
  color: #7f00ff;
}
</style>
