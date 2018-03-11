<template>
  <div class="other-posts">
    <a href="#" class="prev">
      <p class="other-posts__arrow">Previous Post</p>
      <p class="other-posts__title">Lorem ipsum dolor sit amet consectetur adipisicing elit. Omnis veniam dolorem eius modi, consectetur beatae.</p>
    </a>
    <a href="#" class="next">
      <p class="other-posts__arrow">Next Post</p>
      <p class="other-posts__title">Lorem ipsum dolor sit amet, consectetur adipisicing.</p>
    </a>
  </div>
</template>

<style lang="less">
.other-posts {
  display: flex;
  padding: 30px 0;
  border-top: 1px solid #eef0f1;
  justify-content: space-between;

  > a {
    width: 50%;
    text-decoration: none;

    &.prev {
      text-align: left;

      .other-posts__arrow {
        margin-left: 10px;
      }
    }

    &.next {
      text-align: right;

      .other-posts__arrow {
        margin-right: 10px;
      }
    }
  }

  &__arrow {
    font-size: 11px;
    color: #aeb6b9;
    font-style: italic;
    margin-bottom: 10px;
  }

  .other-posts__title {
    font-size: 11px;
    font-weight: bold;
    color: #414648;
    line-height: 1.6;
  }
}
</style>
