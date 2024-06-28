<template>
  <div class="nft-card">
    <div class="nft-description">
      <p class="nft-title">{{ title }}</p>
      <p class="nft-details">{{ details }}</p>
      <p class="nft-price">{{ price }}</p>
    </div>
    <div class="nft-image"><img src="../assets/girl.jpeg" :alt="title" /></div>
  </div>
</template>

<script>
export default {
  name: "NFTCard2",
  props: {
    title: String,
    details: String,
    price: String,
    imageSrc: String,
  },
};
</script>

<style scoped>
.nft-card {
  display: flex;
  flex-direction: row-reverse;
  align-items: center;
  justify-content: space-between;
  background-color: #000;
  color: #fff;
  padding: 20px;
  border: 1px solid #4a4a4a;
  border-radius: 10px;
  

}

.nft-description {
  width: 465px;
  height: 287px;
  margin-right: 20px;
  font-size: 35px;
  line-height: 48px;
  font-weight: 400;
  text-align: left;
}

.nft-title {
  font-size: 1.5rem;
  font-weight: bold;
  margin-bottom: 10px;
}

.nft-details {
  font-size: 1rem;
  margin-bottom: 10px;
}

.nft-price {
  font-size: 1.5rem;
  font-weight: bold;
}

.nft-image img {
    margin-right: 50px;
min-width: 300px;
    max-width: 560px;
    height: 560px;
    border: 2px solid #4a4a4a;
    border-radius: 20px 0px 20px 0px;
}
</style>
