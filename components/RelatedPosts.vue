<template>
  <section class="related-posts">
    <h3 class="title">Related Posts</h3>
    <div class="posts">
      <post
        v-for="post in posts"
        :key="post.id"
        :id="post.id"
        :title="post.title"
        :url="post.url"
      />
    </div>
  </section>
</template>

<script>
import Post from "~/components/Post.vue";

export default {
  components: {
    Post
  },
  props: {
    posts: Array
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
  .posts {
    border-top: 1px solid #eef0f1;
    margin: 15px 0;
    display: flex;
    justify-content: space-between;

    @media (max-width: 600px) {
      display: block;
    }
  }
}
</style>
