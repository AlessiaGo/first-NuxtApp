<template>
  <div class="posts-page">
    <PostList :posts="loadedPosts" />
  </div>
</template>

<script>
import PostList from "@/components/Posts/PostList";

export default {
  components: {
    PostList
  },
  async asyncData(context) {
    try {
const data = await new Promise((resolve, reject) => {
setTimeout(() => {
resolve({
loadedPosts: [
{
id: "1",
title: "First Post",
previewText: "This is our first post!",
thumbnail: "https://static.pexels.com/photos/270348/pexels-photo-270348.jpeg"
},
{
id: "2",
title: "Second Post",
previewText: "This is our second post!",
thumbnail: "https://static.pexels.com/photos/270348/pexels-photo-270348.jpeg"
}
]
});
}, 1000);
});
return data;
} catch (e) {
context.error(e);
}
  }
};
</script>


<style scoped>
.posts-page {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>