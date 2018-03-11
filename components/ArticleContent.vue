<template>
  <section class="article-content">
    <h1 class="article__title">
      What Fashion Editors Are Buying for Every Kid on Our Holiday List
    </h1>
    <p class="article__info">
      <span class="author">John Does</span>
      <span class="date">January 5, 2018</span>
      <span class="comments">11</span>
    </p>
    <img class="article__image" src="/main.png" alt="">
    <p class="article__text">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Doloremque mollitia, tempore nam exercitationem dolores, iure cupiditate cumque amet fuga est tenetur error voluptate saepe quas molestias beatae, consequuntur porro debitis nobis eos! Eaque, rerum nesciunt ipsa provident est reiciendis error natus impedit, modi nam nisi id voluptatibus cupiditate, molestiae ullam.</p>
    <h2 class="article__subtitle">Lorem, ipsum dolor sit amet consectetur adipisicing elit. Voluptas, nobis.</h2>
    <p class="article__text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda molestiae quam hic repellat laudantium illo in, omnis corrupti illum deleniti labore corporis, ab magni modi mollitia eaque suscipit dolorem nostrum? Nemo deserunt vitae unde iure quae voluptatum consectetur ratione, facere perspiciatis ex repellendus. Alias, sequi. Iure autem aliquid molestiae eum distinctio laboriosam facere consequuntur veniam qui, rerum sed, at error libero. Quos doloribus eligendi eos, sapiente quae unde voluptatum ex neque voluptate tenetur officiis quasi, asperiores sunt quo vero excepturi saepe? Dolorem id quidem ratione asperiores nostrum, optio saepe provident accusantium veniam ut aliquid expedita nemo sunt excepturi tempora tenetur.</p>
    <h4 class="about-author">About Author</h4>
    <div class="about">
      <img class="about__avatar" src="https://lorempixel.com/50/50/people/3/" alt="">
      <div class="about__body">
        <p class="about__author">John Does</p>
        <p class="about__text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis nobis voluptas nulla adipisci aperiam at velit facilis, doloribus totam minus, consequatur atque optio harum corporis esse tenetur nisi quaerat deleniti explicabo dolorem odio ut. Unde ratione sit omnis aspernatur dignissimos?</p>
      </div>
    </div>
    <div class="other-posts">
      <div class="prev">
        <p class="other-posts__arrow">Previous Post</p>
        <p class="other-posts__title">Lorem ipsum dolor sit amet consectetur adipisicing elit. Omnis veniam dolorem eius modi, consectetur beatae.</p>
      </div>
      <div class="next">
        <p class="other-posts__arrow">Next Post</p>
        <p class="other-posts__title">Lorem ipsum dolor sit amet, consectetur adipisicing.</p>
      </div>
    </div>
  </section>
</template>

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

  .about-author {
    color: #414648;
    margin: 20px 0 15px;
    padding-top: 30px;
    font-size: 18px;
    border-top: 1px solid #eef0f1;
  }

  .about {
    display: flex;
    padding: 30px 0;
    border-top: 1px solid #eef0f1;

    &__avatar {
      display: block;
      border-radius: 25px;
      width: 50px;
      height: 50px;
    }

    &__body {
      margin-left: 25px;
      width: calc(100% - 75px);
    }

    &__author {
      font-weight: bold;
      text-transform: uppercase;
      margin-bottom: 10px;
      font-size: 14px;
      color: #5f6365;
    }

    &__text {
      color: #878c8e;
      font-size: 14px;
      line-height: 1.6;
    }

  }

  .other-posts {
    display: flex;
    padding: 30px 0;
    border-top: 1px solid #eef0f1;
    justify-content: space-between;

    > div {
      width: 50%;

      &.prev {
        text-align: left;
      }

      &.next {
        text-align: right;
      }
    }

    &__arrow {
      font-size: 11px;
      color: #aeb6b9;
      font-style: italic;
      margin-bottom: 10px;

      &.prev {
        margin-left: 10px;
      }

      &.next {
        margin-right: 10px;
      }
    }

    .other-posts__title {
      font-size: 11px;
      font-weight: bold;
      color: #414648;
      line-height: 1.6;
    }

  }
}
</style>
