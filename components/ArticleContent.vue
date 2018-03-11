<template>
  <section class="article-content">
    <h1 class="article__title">
      What Fashion Editors Are Buying for Every Kid on Our Holiday List
    </h1>
    <p class="article__info">
      <img class="icon" src="user.svg" alt="">
      <span class="author">John Does</span>
      <img class="icon" src="calendar-page-empty.svg" alt="">
      <span class="date">January 5, 2018</span>
      <img class="icon" src="speech-bubbles-comment-option.svg" alt="">
      <span class="comments">{{ commentsCount }}</span>
    </p>
    <img class="article__image" src="/main.png" alt="">
    <p class="article__text">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Doloremque mollitia, tempore nam exercitationem dolores, iure cupiditate cumque amet fuga est tenetur error voluptate saepe quas molestias beatae, consequuntur porro debitis nobis eos! Eaque, rerum nesciunt ipsa provident est reiciendis error natus impedit, modi nam nisi id voluptatibus cupiditate, molestiae ullam.</p>
    <h2 class="article__subtitle">{{ article.title }}</h2>
    <p class="article__text">{{ article.body }}</p>
    <about-author />
    <other-posts />
  </section>
</template>

<script>
import OtherPosts from "~/components/OtherPosts.vue";
import AboutAuthor from "~/components/AboutAuthor.vue";

export default {
  components: {
    AboutAuthor,
    OtherPosts
  },
  props: {
    commentsCount: Number,
    article: Object
  }
};
</script>

<style lang="less">
.article-content {
  margin: 20px 0 40px;
  border-bottom: 1px solid #eef0f1;

  .article__title {
    color: #414648;
    font-size: 34px;
  }

  .article__info {
    margin: 10px 0 5px;

    span {
      font-size: 11px;
      color: #aeb6b9;
      margin: 0 15px 0 5px;
    }
  }

  .article__text {
    color: #929698;
    line-height: 1.6;
    font-size: 14px;
    margin: 10px 0;
  }

  .article__subtitle {
    color: #414648;
    line-height: 1.6;
    font-size: 24px;
    text-transform: capitalize;
  }

  .article__image {
    width: 100%;
    margin: 20px 0;
  }
}
</style>
