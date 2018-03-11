<template>
  <div>
    <h4 class="about-author">About Author</h4>
    <div class="about">
      <img class="about__avatar" src="https://lorempixel.com/50/50/cats/7/" alt="">
      <div class="about__body">
        <p class="about__author">John Does</p>
        <p class="about__text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis nobis voluptas nulla adipisci aperiam at velit facilis, doloribus totam minus, consequatur atque optio harum corporis esse tenetur nisi quaerat deleniti explicabo dolorem odio ut. Unde ratione sit omnis aspernatur dignissimos?</p>
      </div>
    </div>
  </div>
</template>

<style lang="less">
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
</style>