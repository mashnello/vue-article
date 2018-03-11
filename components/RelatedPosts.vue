<template>
  <section class="related-posts">
    <h3 class="title">Related Posts</h3>
    <div class="posts">
      <post />
      <post />
      <post />
    </div>
  </section>
</template>

<script>
import Post from "~/components/Post.vue";

export default {
  components: {
    Post
  }
};
</script>

<style lang="less">
.related-posts {
  margin: 20px 0;

  .title {
    color: #464c4e;
    text-transform: uppercase;
    margin: 15px 0;
  }
}
</style>
