<template>
  <a href="#" class="post">
    <img class="post__image" :src="'https://lorempixel.com/600/300/cats/' + id + '/'" alt="">
    <h4 class="post__title">{{ title }}</h4>
    <p class="post__info">
      <img class="icon" src="user.svg" alt="">
      <span class="post__author">John Does</span>
      <img class="icon" src="calendar-page-empty.svg" alt="">
      <span class="post__date">January 15, 2018</span>
    </p>
  </a>
</template>

<script>
export default {
  props: {
    id: Number,
    url: String,
    title: String
  }
};
</script>

<style lang="less">
.post {
  margin: 30px 0;
  width: 32%;
  text-decoration: none;
  display: block;

  @media (max-width: 600px) {
    width: 100%;
  }

  &__image {
    width: 100%;
    height: 170px;
  }

  &__title {
    color: #484c4e;
    margin: 20px 0;
    line-height: 1.6;
    font-size: 12px;
    text-transform: capitalize;
  }

  &__info {
    display: flex;
    justify-content: flex-start;
    color: #929698;
    font-size: 10px;

    span {
      margin: 0 15px 0 5px;
    }
  }
}
</style>
