<template>
      <section class="posts-list">
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
</template>

<script>
import PostPreview from '../../components/Posts/PostPreview.vue';

export default{
  components:{
    PostPreview : PostPreview
  }
}
</script>

<style scoped>
.posts-list {
  display: flex;
  padding: 20px;
  box-sizing: border-box;
  flex-wrap: wrap;
  align-items: center;
  justify-content: center;
}
</style>