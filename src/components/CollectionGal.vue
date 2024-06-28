<template>
  <div class="collections">
    <h2 style="text-align: left; margin: 30px; font-size: 40px">Collections</h2>
    <div class="gallery-wrapper">
      <button class="scroll-btn left" @click="scrollLeft">&lt;</button>
      <div class="gallery" ref="gallery">
        <div
          class="card"
          v-for="(collection, index) in collections"
          :key="index"
        >
          <img :src="collection.image" alt="" />
          <div class="info">
            <p>{{ collection.name }}</p>
            <span>Floor: {{ collection.floor }}</span>
          </div>
        </div>
      </div>
      <button class="scroll-btn right" @click="scrollRight">&gt;</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "CollectionsGal",
  data() {
    return {
      collections: [
        {
          image: require("../assets/col1.jpeg"),
          name: "XO Girls NFT Collection",
          floor: "0.07 ETH",
        },
        {
          image: require("../assets/col2.png"),
          name: "Game character 3d Collection",
          floor: "0.05 ETH",
        },
        {
          image: require("../assets/col3.jpeg"),
          name: "Monkey Collections",
          floor: "0.01 ETH",
        },
        {
          image: require("../assets/col4.jpeg"),
          name: "PROJECT NFT cub",
          floor: "0.07 ETH",
        },
        // Add more collections as needed
      ],
    };
  },
  methods: {
    scrollLeft() {
      this.$refs.gallery.scrollBy({ left: -315, behavior: "smooth" });
    },
    scrollRight() {
      this.$refs.gallery.scrollBy({ left: 315, behavior: "smooth" });
    },
  },
};
</script>

<style scoped lang="scss">
.collections {
  position: relative;
  padding: 20px;
}

.gallery-wrapper {
  position: relative;
  display: flex;
  align-items: center;
}

.gallery {
  display: flex;
  overflow-x: auto;
  padding: 20px;
  scroll-behavior: smooth;
}

.card {
  position: relative;
  width: 315px;
  height: 314px;
  border-radius: 16px;
  margin-right: 20px;
  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 16px;
  }
  .info {
    background-color: rgba(0, 0, 0, 0.75);
    font-size: 16px;
    color: #ffffff;
    height: 69px;
    width: 100%;
    position: absolute;
    bottom: 0;
    border-bottom-left-radius: 16px;
    border-bottom-right-radius: 16px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
}

.scroll-btn {
  background-color: #712b9d;
  color: #ffffff;
  font-size: 25px;
  border: none;
  border-radius: 50%;
  width: 40px;
  height: 40px;
  cursor: pointer;
  position: absolute;
  z-index: 10;
  transition: background-color 0.3s;
}

.scroll-btn.left {
  left: 10px;
}

.scroll-btn.right {
  right: 10px;
}

.scroll-btn:hover {
  background-color: #561d75;
}

h2 {
  font-size: 2.5em;
  margin-bottom: 20px;
  color: #ffffff;
}
</style>
