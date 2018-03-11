<template>
  <main class="main">
    <article-content />
    <related-articles />
    <article-comments />
  </main>
</template>

<script>
import ArticleContent from "~/components/ArticleContent.vue";
import RelatedArticles from "~/components/RelatedArticles.vue";
import ArticleComments from "~/components/ArticleComments.vue";

export default {
  components: {
    ArticleContent,
    RelatedArticles,
    ArticleComments
  }
};
</script>