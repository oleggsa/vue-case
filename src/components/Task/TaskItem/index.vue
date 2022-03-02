<template>
  <div class="task__item">
    <div class="task__header">
      <img src="./../../../../images/task-header.png" alt="img">
      <p>{{taskListItem.id}}</p>
    </div>
    <div class="task__text">
      {{taskListItem.text}}
    </div>
    <div class="task__img">
      <img :src="taskListItem.img" alt="img">
    </div>
  </div>
</template>

<script>
export default {
  name: "index",
  props: {
    taskListItem: {
      type: Object
    }
  }
}
</script>

<style lang="scss" scoped>
.task {
  &__item {
    display: inline-block;
    max-width: 460px;
    max-height: 340px;
    position: relative;
    margin-bottom: 105px;
  }
  &__header {
    & p{
      position: absolute;
      font-family: 'Roboto', sans-serif;
      font-weight: bold;
      font-size: 100px;
      color: #0087E0;
      top: -103px;
      left: 23px;
    }
    & img{
      width: 100%;
    }
  }
  &__text {
    position: absolute;
    left: 122px;
    top: 49px;
    font-weight: 500;
    font-size: 18px;
    color: white;
  }
  &__img {
    text-align: right;
    margin-top: 12px;
  }
}

@media (max-width: 992px) {
  .task {
    &__item {
      width: 49%;
      margin-bottom: 28px;
      &:nth-child(odd) {
        margin-right: 3px;
      }
    }
    &__header {
      & p {
        font-size: 10vw;
        top: -10vw;
        left: 2.5vw;
      }
    }
    &__text {
      top: 4vw;
      left: 12vw;
    }
    &__img {
      text-align: right;
      margin-top: 12px;
      & img {
        width: 78%;
      }
    }
  }
}

@media (max-width: 768px) {
  .task {
    &__text {
      font-size: 2.5vw;
    }
    &__img {
      margin-top: 20px;
    }
  }
}

@media (max-width: 576px) {
  .task {
    &__text {
      font-size: 14px;
      line-height: 110%;
      font-weight: normal;
    }
    &__img {
      margin-top: 46px;
      & img {
        max-height: 252px;
      }
    }
  }
}
</style>