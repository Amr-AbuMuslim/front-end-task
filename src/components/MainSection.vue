<template>
  <section class="main-section">
    <div class="content">
      <h1>Your own NFT Market place without Coding</h1>
      <p class="main-text">
        The fastest and easiest way to fully unlock the potential of your
        digital assets. Create and run an exclusive marketplace for your NFT
        business today!
      </p>
      <div class="email-signup">
        <input type="email" placeholder="Enter your email..." />
        <button>Start Free</button>
      </div>
    </div>
    <footer>
      <h2>Powering leading brands</h2>
      <h2>Coindesk</h2>
      <h2>H E F T Y V E R S E</h2>
    </footer>
  </section>
</template>

<script>
export default {
  name: "MainSection",
};
</script>

<style lang="scss" scoped>
.main-section {
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  height: 100vh;
  margin-top: -80px;
  background: linear-gradient(to bottom, rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)),
    url("../assets/landing.jpeg");
  background-size: cover;
  background-repeat: no-repeat;
  text-align: center;
  color: #fff;
  padding: 0 20px;
}

.content {
  max-width: 600px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

h1 {
  font-size: 48px;
  font-weight: 700;
  line-height: 72px;
  width: 677px;
}

.main-text {
  font-size: 16px;
  font-weight: 400;
  line-height: 24px;
  width: 497px;
  margin: 30px;
}

.email-signup {
  display: flex;
  justify-content: center;
  gap: 20px;
}

.email-signup input {
  padding: 8px;
  font-size: 15px;

  border: none;
  border-radius: 16px;
  background-color: #00000083;
  width: 272px;
}

.email-signup button {
  padding: 10px 20px;
  font-size: 15px;
  border: none;
  background-color: #8000ff71;
  color: #fff;

  border-radius: 16px;
  cursor: pointer;
}

.email-signup button:hover {
  background-color: #5900b3;
}
.tape {
}
footer {
  background-color: #816797;
  position: absolute;
  bottom: 0px;
  height: 83px;
  width: 100%;
  display: flex;
  justify-content: space-around;
  gap: 20px;
  h2 {
    margin-top: 20px;
  }
}
</style>
