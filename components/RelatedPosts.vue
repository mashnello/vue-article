<template>
  <section class="related-posts">
    <div class="title-wrapper">
      <h3 class="title">
        Related Posts
      </h3>
      <span class="controls">
        <button class="controls__button prev" @click="prev">
          <img class="icon" src="left-arrow.svg" alt="">
        </button>
        <button class="controls__button next" @click="next">
          <img class="icon" src="right-arrow.svg" alt="">
        </button>
      </span>
    </div>
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
    articles: Array
  },
  data() {
    return {
      posts: this.articles.slice()
    }
  },
  methods: {
    next() {
      const first = this.posts.shift();
      this.posts = this.posts.concat(first);
    },
    prev() {
      const last = this.posts.pop();
      this.posts = [last].concat(this.posts);
    }
  }
};
</script>

<style lang="less">
.related-posts {
  display: flex;
  flex-direction: column;
  margin: 20px 0;

  .title-wrapper {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;

    .title {
      color: #464c4e;
      text-transform: uppercase;
    }

    .controls__button {
      border: 1px solid #eef0f1;
      margin-left: 3px;
      width: 25px;
      height: 25px;
    }
  }

  .posts {
    display: flex;
    overflow: hidden;
    width: 100%;
    height: 330px;
    flex-wrap: wrap;
    justify-content: space-between;
    border-top: 1px solid #eef0f1;
    margin: 15px 0;

    @media (max-width: 600px) {
      display: block;
    }
  }
}
</style>
