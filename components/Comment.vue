<template>
  <div :class="'comment ' + (id % 2 ? '' : 'replied')">
    <img class="comment__avatar" :src="'https://lorempixel.com/50/50/cats/' + id + '/'" alt="">
    <div class="comment__content">
      <p class="comment__author">{{ name }}</p>
      <p class="comment__date">January 5, 2018 at 6:02 am</p>
      <p class="comment__text">{{ body }}</p>
      <button class="comment__button">Reply</button>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    id: Number,
    name: String,
    body: String
  }
}
</script>

<style lang="less">
.comment {
  display: flex;
  padding: 30px 0;
  border-top: 1px solid #eef0f1;

  &.replied {
    margin-left: 55px;
  }

  &__avatar {
    display: block;
    border-radius: 25px;
    width: 50px;
    height: 50px;
  }

  &__content {
    margin-left: 15px;
    width: calc(100% - 65px);
  }

  &__author {
    font-weight: bold;
    margin-bottom: 10px;
    font-size: 14px;
    color: #5f6365;
  }

  &__date {
    font-style: italic;
    margin-bottom: 15px;
    font-size: 11px;
    color: #aeb6b9;
  }

  &__text {
    color: #878c8e;
    font-size: 14px;
    line-height: 1.6;
    margin-bottom: 15px;
  }

  &__button {
    background-color: #e2e2e4;
    color: #222222;
    font-size: 14px;
    padding: 5px 10px;
    border-radius: 4px;
    border: 0;
    cursor: pointer;
  }
}
</style>
