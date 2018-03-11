<template>
  <main class="main">
    <article-content />
    <related-posts />
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
    const { data } = await axios.get('https://jsonplaceholder.typicode.com/comments?postId=1')
    return { comments: data }
  }
};
</script>

<style>
.main {
  max-width: 700px;
}
</style>
