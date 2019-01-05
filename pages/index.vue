<template>
<div class="home-page">
  <section class="intro">
    <h1>Get the latest tech news</h1>
  </section>
  <section class="featured-posts">
    <PostPreview 
       id="1" 
       thumbnail="https://d32r1sh890xpii.cloudfront.net/article/718x300/93728e7f7f7483493cc49df735861759.jpg" 
       title="Hello there!"
       previewText="Preview text"/>
    <PostPreview 
       id="2" 
       thumbnail="https://d32r1sh890xpii.cloudfront.net/article/718x300/93728e7f7f7483493cc49df735861759.jpg" 
       title="Hello there! 2"
       previewText="Preview text 2"/>
    <PostPreview 
      id="3" 
      thumbnail="https://d32r1sh890xpii.cloudfront.net/article/718x300/93728e7f7f7483493cc49df735861759.jpg" 
      title="Hello there! 3"
      previewText="Preview text 3"/>
  </section>
</div>
</template>

<script>
import PostPreview from '@/components/Posts/PostPreview'

export default {
  components: {
    PostPreview
  }
}
</script>

<style scoped>
.intro {
  height: 300px;
  position: relative;
  padding: 30px;
  box-sizing: border-box;
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
</style>
