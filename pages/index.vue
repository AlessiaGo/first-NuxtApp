<template>
  <div class="home-page">
    <section class="intro">
      <h1>Get the latest tech news!</h1>
    </section>
    <section class="featured-posts">
      <PostPreview
        id="1"
        thumbnail="https://images.unsplash.com/photo-1535350356005-fd52b3b524fb?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1170&q=80"
        title="Hello"
        preview-text="These is my first post"/>
      <PostPreview
        id="2"
        thumbnail="https://img.freepik.com/free-vector/composed-particles-swirling-abstract-graphics_456031-137.jpg?w=2000&t=st=1692885798~exp=1692886398~hmac=4d0e7583442c46a09cbb434450c10fcb3dd6f760d57969b4f180519ac68c2c12"
        title="Hello"
        preview-text="This is my second post"
      />
      <PostPreview
        id="3"
        thumbnail="https://media.istockphoto.com/id/1305012465/it/vettoriale/connessione-internet-senso-astratto-della-scienza-e-della-tecnologia-illustrazione.jpg?s=612x612&w=0&k=20&c=r9U1QleziK9ptof9-cWY--AKQ9lt4MV055D9NBA3AF8="
        title="Hello"
        preview-text="This is my third post"
      />
    </section>
  </div>
</template>

<script>
import PostPreview from '../components/Posts/PostPreview.vue';

export default{
  components:{
    PostPreview : PostPreview
  }
}
</script>

<style scoped>
.intro {
  height: 300px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
  background-image: url('../assets/images/main-page-background.jpg');
  background-position: center;
  background-size: cover;
}

.intro h1 {
  position: absolute;
  top: 10%;
  left: 5%;
  width: 90%;
  font-size: 1.5rem;
  color: black;
  background-color: rgb(211, 211, 211);
  padding: 10px;
  border-radius: 10px;
  box-shadow: 3px 3px 3px black;
  box-sizing: border-box;
  border: 1px solid black;
}

@media (min-width: 768px) {
  .intro h1 {
    font-size: 2rem;
  }
}

.featured-posts {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}

.post-preview {
  border: 1px solid #ccc;
  box-shadow: 0 2px 2px #ccc;
  background-color: white;
  width: 90%;
}

a {
  text-decoration: none;
  color: black;
}

@media (min-width: 850px) {
  .post-preview {
    width: 400px;
    margin: 10px;
  }
}

.post-thumbnail {
  width: 100%;
  height: 200px;
  background-position: center;
  background-size: cover;
}

.post-content {
  padding: 10px;
  text-align: center;
}

a:hover .post-content,
a:active .post-content {
  background-color: #ccc;
}
</style>
