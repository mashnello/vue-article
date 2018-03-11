<template>
  <section class="article-content">
    <h1 class="article__title">
      What Fashion Editors Are Buying for Every Kid on Our Holiday List
    </h1>
    <p class="article__info">
      <span class="author">John Does</span>
      <span class="date">January 5, 2018</span>
      <span class="comments">5</span>
    </p>
    <img class="article__image" src="/main.png" alt="">
    <p class="article__text">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Doloremque mollitia, tempore nam exercitationem dolores, iure cupiditate cumque amet fuga est tenetur error voluptate saepe quas molestias beatae, consequuntur porro debitis nobis eos! Eaque, rerum nesciunt ipsa provident est reiciendis error natus impedit, modi nam nisi id voluptatibus cupiditate, molestiae ullam.</p>
    <h2 class="article__subtitle">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Voluptas, nobis.</h2>
    <p class="article__text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda molestiae quam hic repellat laudantium illo in, omnis corrupti illum deleniti labore corporis, ab magni modi mollitia eaque suscipit dolorem nostrum? Nemo deserunt vitae unde iure quae voluptatum consectetur ratione, facere perspiciatis ex repellendus. Alias, sequi. Iure autem aliquid molestiae eum distinctio laboriosam facere consequuntur veniam qui, rerum sed, at error libero. Quos doloribus eligendi eos, sapiente quae unde voluptatum ex neque voluptate tenetur officiis quasi, asperiores sunt quo vero excepturi saepe? Dolorem id quidem ratione asperiores nostrum, optio saepe provident accusantium veniam ut aliquid expedita nemo sunt excepturi tempora tenetur.</p>
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
      margin-left: 20px;
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
  }

  .article__image {
    width: 100%;
    margin: 20px 0;
  }
}
</style>
