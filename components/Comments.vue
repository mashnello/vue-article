<template>
  <section class="comments-wrapper">
    <h3 class="title">5 Comments</h3>
    <div class="comments">
      <comment
        v-for="comment in comments"
        :key="comment.id"
        :id="comment.id"
        :name="comment.name"
        :body="comment.body"
      />
    </div>
  </section>
</template>

<script>
import Comment from "~/components/Comment.vue";

export default {
  components: {
    Comment
  },
  props: {
    comments: Array
  }
};
</script>

<style lang="less">
.comments-wrapper {
  margin: 20px 0;

  .title {
    color: #464c4e;
    text-transform: uppercase;
    margin: 15px 0;
  }
}
</style>
