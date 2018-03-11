<template>
  <section class="related-articles">
    <h3 class="title">Related Posts</h3>
    <div class="posts">
      <div class="post">
        <img class="post__image" src="https://lorempixel.com/600/300/fashion/1" alt="">
        <h4 class="post__title">Lorem ipsum dolor sit amet consectetur adipisicing elit. Non, alias!</h4>
        <p class="post__info">
          <span class="post__author">John Does</span>
          <span class="post__date">January 15, 2018</span>
        </p>
      </div>
      <div class="post">
        <img class="post__image" src="https://lorempixel.com/600/300/fashion/5" alt="">
        <h4 class="post__title">Lorem ipsum dolor sit amet consectetur adipisicing elit. Non, alias!</h4>
        <p class="post__info">
          <span class="post__author">John Does</span>
          <span class="post__date">January 15, 2018</span>
        </p>
      </div>
      <div class="post">
        <img class="post__image" src="https://lorempixel.com/600/300/fashion/10" alt="">
        <h4 class="post__title">Lorem ipsum dolor sit amet consectetur adipisicing elit. Non, alias!</h4>
        <p class="post__info">
          <span class="post__author">John Does</span>
          <span class="post__date">January 15, 2018</span>
        </p>
      </div>
    </div>
  </section>
</template>

<style lang="less">

.related-articles {
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

    .post {
      margin: 30px 0;
      width: 32%;

      &__image {
        width: 100%;
        height: 170px;
      }

      &__title {
        color: #484c4e;
        margin: 20px 0;
        line-height: 1.6;
        font-size: 12px;
      }

      &__info {
        display: flex;
        justify-content: flex-start;
        color: #929698;
        font-size: 10px;

        span {
          margin: 0 10px;
        }
      }

    }
  }
}

</style>
