<template>
  <main class="main">
    <article-content :article="article" :commentsCount="comments.length" />
    <related-posts :posts="posts" />
    <comments :comments="comments" />
  </main>
</template>

<script>
import axios from 'axios';
import ArticleContent from "~/components/ArticleContent.vue";
import RelatedPosts from "~/components/RelatedPosts.vue";
import Comments from "~/components/Comments.vue";

export default {
  components: {
    ArticleContent,
    RelatedPosts,
    Comments
  },
  async asyncData () {
    const article = await axios.get('https://jsonplaceholder.typicode.com/posts/1');
    const posts = await axios.get('https://jsonplaceholder.typicode.com/photos/');
    const comments = await axios.get('https://jsonplaceholder.typicode.com/posts/1/comments');

    return {
      article: article.data,
      posts: posts.data.slice(5, 8),
      comments: comments.data
    }
  }
};
</script>

<style>
.main {
  max-width: 700px;
}
</style>
