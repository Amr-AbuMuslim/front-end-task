<template>
  <div class="collections">
    <h2 style="text-align: left ; margin:30px; font-size:40px">Collections</h2>
    <div class="gallery">
      <div class="card">
        <img src="../assets/col1.jpeg" alt="" />
        <div class="info">
          <p>XO Girls NFT Collection</p>
          <span>Floor: 0.07 ETH</span>
        </div>
      </div>
      <div class="card">
        <img src="../assets/col2.png" alt="" />
        <div class="info">
          <p>Game character 3d Collection</p>
          <span>Floor: 0.05 ETH</span>
        </div>
      </div>
      <div class="card">
        <img src="../assets/col3.jpeg" alt="" />
        <div class="info">
          <p>Monkey Collections</p>
          <span>Floor : 0.01 ETH</span>
        </div>
      </div>
      <div class="card">
        <img src="../assets/col4.jpeg" alt="" />
        <div class="info">
          <p>PROJECT NFT cub</p>
          <span>Floor: 0.07 ETH</span>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "CollectionsGal",
};
</script>
<style lang="scss">
.gallery {
  padding: 20px;
  display: flex;
  justify-content: space-between;
}
.card {
  position: relative;
  width: 315px;
  height: 314px;
  border-radius: 16px;
  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  p {
  }
}
.info {
  background-color: #000000bf;
  margin-top: -70px;
  font-size: 16px;
  color: #ffffff;
  height: 69px;
  width: 100%;
  position: absolute;
}
</style>
