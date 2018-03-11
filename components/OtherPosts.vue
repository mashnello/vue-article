<template>
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
</template>

<style lang="less">
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
</style>
