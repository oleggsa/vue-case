<template>
  <div class="stack">
    <div class="container">
      <div class="stack__content">
        <div class="header">Technology Stack</div>
        <div class="header header-media">Tech Stack</div>
        <div class="stack__first-row">
          <div class="stack__first-row-image"><img src="./../../../images/stack-1.png" alt="stack1"></div>
          <div class="stack__first-row-image"><img src="./../../../images/stack-2.png" alt="stack2"></div>
          <div class="stack__first-row-image"><img src="./../../../images/stack-3.png" alt="stack3"></div>
        </div>
        <div class="stack__second-row">
          <div class="stack__second-row-image"><img src="./../../../images/stack-4.png" alt="stack4"></div>
          <div class="stack__second-row-image"><img src="./../../../images/stack-5.png" alt="stack5"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "index"
}
</script>

<style lang="scss" scoped>
.stack {
  margin-top: 46px;
  &__content {
    text-align: center;
    & .header {
      color: #51ACEA;
      &-media {
        display: none;
      }
    }
   }
  &__first-row {
    margin-top: 95px;
    display: flex;
    justify-content: center;
    & div {
      width: 240px;
      &:first-child img{
        padding-top: 26px;
      }
      &:last-child img{
        padding-top: 5px;
      }
    }
  }
  &__second-row {
    display: flex;
    justify-content: center;
    margin-top: 61px;
    & div {
      width: 360px;
      &:last-child img {
        padding: 17px;
      }
    }
  }
}

@media (max-width: 576px) {
  .stack {
    &__content {
      margin: 10px;
      & .header {
        display: none;
        &-media {
          display: block;
          font-size: 56px;
        }
      }
    }
    &__first-row {
      margin-top: 40px;
      & div:nth-child(1) {
        padding-top: 50px;
        & img{
          height: 56px;
          width: 118px;
          vertical-align: bottom;
          padding: 0;
        }
      }
      & div:nth-child(2) {
        padding-top: 24px;
        & img{
          height: 56px;
          width: 81px;
          margin-top: 26px;
        }
      }
      & div:nth-child(3) {
        padding-top: 24px;
        & img {
          height: 66px;
          width: 112px;
          margin-top: 17px;
        }
      }
    }
    &__second-row {
      margin-top: 46px;
      & div:first-child {
        & img {
          width: 56px;
          height: 56px;
          margin-right: 3px;
        }
      }
      & div:last-child {
        & img {
          padding: 0 12px;
        }
      }
    }
  }
}
</style>