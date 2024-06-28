<template>
  <div class="about">
    <h1>About Us</h1>
    <div class="posts-container">
      <div v-for="post in posts" :key="post.id" class="post">
        <h2>{{ post.title }}</h2>
        <p>{{ post.body }}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      posts: [],
    };
  },
  created() {
    fetch("https://jsonplaceholder.typicode.com/posts")
      .then((response) => response.json())
      .then((data) => {
        this.posts = data.slice(0, 5); // Limiting to 5 posts for display
      });
  },
};
</script>

<style scoped>
.about {
  color: white;
  background-color: #712b9d;
  padding: 40px 20px;
  border-radius: 10px;
  text-align: center;
  max-width: 1200px;
  margin: auto;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}

.posts-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  margin-top: 20px;
}

.post {
  background: rgba(255, 255, 255, 0.1);
  padding: 20px;
  margin: 10px;
  border-radius: 10px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  flex: 1 1 30%;
  max-width: 30%;
  transition: transform 0.3s, box-shadow 0.3s;
}

.post:hover {
  transform: translateY(-10px);
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
}

h1 {
  font-size: 2.5em;
  margin-bottom: 20px;
}

h2 {
  font-size: 1.8em;
  margin-bottom: 10px;
}

p {
  font-size: 1.2em;
}
</style>
