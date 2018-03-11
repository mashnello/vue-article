<template>
  <main class="main">
    <article-content />
    <related-posts />
    <comments />
  </main>
</template>

<script>
import ArticleContent from "~/components/ArticleContent.vue";
import RelatedPosts from "~/components/RelatedPosts.vue";
import Comments from "~/components/Comments.vue";

export default {
  components: {
    ArticleContent,
    RelatedPosts,
    Comments
  }
};
</script>

<style>
.main {
  max-width: 700px;
}
</style>
