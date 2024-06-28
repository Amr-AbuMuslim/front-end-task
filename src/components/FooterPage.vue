<template>
  <footer class="footer">
    <div class="divider">
      <div class="newsletter">
        <h2>Join our weekly digest!</h2>
        <p>Get exclusive promotions & updates straight to your inbox.</p>
        <div class="newsletter-form">
          <div class="register">
            <input type="email" placeholder="Enter your email..." />
            <button class="subscribe-btn">Subscribe</button>
          </div>
          <button class="create-store-btn">Create Free Store</button>
        </div>
      </div>
      <div class="footer-links">
        <div class="footer-column">
          <h3>FEATURES</h3>
          <ul>
            <li>Build Store</li>
            <li>Sell NFT</li>
            <li>Grow Business</li>
          </ul>
        </div>
        <div class="footer-column">
          <h3>SERVICES</h3>
          <ul>
            <li>Concierge</li>
            <li>Customization</li>
          </ul>
        </div>
        <div class="footer-column">
          <h3>PRODUCT</h3>
          <ul>
            <li>About Us</li>
            <li>Whitepaper</li>
            <li>$N1 Token</li>
            <li>Directory</li>
          </ul>
        </div>
        <div class="footer-column">
          <h3>RESOURCES</h3>
          <ul>
            <li>Help Center</li>
            <li>NFTify Branding</li>
            <li>Success Stories</li>
            <li>Video Tutorials</li>
            <li>Contact Support</li>
          </ul>
        </div>
      </div>
    </div>
    <hr
      style="
        background-color: #816797;
        border: none;
        height: 2px;
        margin-bottom: 30px;
      "
    />
    <div class="footer-bottom">
      <h2>The Leading No-code NFT Marketplace Solution</h2>
      <div class="footer-info">
        <p>© Copyright NFTify Network. All Rights Reserved.</p>
        <div class="social-icons">
          <i class="fab fa-twitter"></i>
          <i class="fab fa-telegram"></i>
          <i class="fab fa-facebook"></i>
          <i class="fab fa-linkedin"></i>
          <i class="fab fa-instagram"></i>
        </div>
        <p>Terms of Service</p>
        <p>Privacy Policy</p>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterPage",
};
</script>

<style lang="scss" scoped>
.footer {
  background: linear-gradient(180deg, #52057b 0%, #000000 100%);

  color: white;
  padding: 40px 20px;
}
.divider {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 20px;
}
.newsletter {
  text-align: left;
  margin-bottom: 60px;
  padding: 20px;
  color: #d6d5a8;
}

.newsletter h2 {
  font-size: 28px;
  font-weight: 600;
  line-height: 42px;
  margin-bottom: 10px;
}

.newsletter p {
  font-size: 16px;
  font-weight: 400;
  width: 367px;
  margin-bottom: 20px;
}

.newsletter-form {
  display: flex;
  justify-content: center;
  align-items: left;
  flex-direction: column;
  margin-bottom: 20px;
}

.newsletter-form input {
  padding: 7px;
  margin-right: 20px;
  width: 272px;
  background-color: #00000060;
  border-radius: 16px;
  border: none;
}

.newsletter-form .subscribe-btn {
  cursor: pointer;
  font-size: 15px;
  font-weight: 400;
  padding: 7px;
  width: 111px;
  background-color: #000000;
  border-radius: 16px;
  color: white;
  border: none;
}

.create-store-btn {
  cursor: pointer;
  padding: 10px 20px;
  border-radius: 16px;
  background-color: #712b9d;
  margin-top: 20px;
  width: 160px;
  color: white;
  border: none;
}

.footer-links {
  flex: 1;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(70px, 1fr));
  margin-left: 50px;
  font-weight: 300;
  color: #d6d5a8;
  //   margin-bottom: 20px;
}

.footer-column h3 {
  margin-bottom: 10px;
  font-weight: 700;
  text-align: left;
}

.footer-column ul {
  list-style: none;
  padding: 0;
  margin: 0px;
  text-align: left;
}

.footer-column li {
  margin-bottom: 25px;
  font-weight: 300;
}

.footer-bottom {
  text-align: center;
  padding: 2px;
  h2 {
    margin-bottom: 40px;
    font-size: 20px;
    font-weight: 500;
  }
  p {
    font-size: 12px;
    font-weight: 400;
  }
}

.footer-bottom .social-icons {
  display: flex;
  justify-content: space-between;
  gap: 30px;
}

.footer-bottom .social-icons i {
  font-size: 25px;
  border: 1px solid #ffffff80;
  color: #ffffff80;
  padding: 7px;
  border-radius: 5px;
}
.footer-info {
  display: flex;
  justify-content: space-around;
  align-items: center;
  h2 {
    margin: 0px;
    padding: 0px;
  }
}
</style>
