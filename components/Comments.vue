<template>
  <section class="comments-wrapper">
    <h3 class="title">5 Comments</h3>
    <div class="comments">
      <comment />
      <comment class="replied" />
      <comment class="replied" />
      <comment />
      <comment />
    </div>
  </section>
</template>

<script>
import Comment from "~/components/Comment.vue";

export default {
  components: {
    Comment
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
