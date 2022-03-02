<template>
  <div class="approach__item">
    <img :src="ApproachListItem.img" alt="img">
    <div class="approach__text">
      {{ApproachListItem.text}}
    </div>
  </div>
</template>

<script>
export default {
  name: "index",
  props: {
    ApproachListItem: {
      type: Object
    }
  }
}
</script>

<style lang="scss" scoped>
.approach {
  &__item {
    margin-top: 16px;
    display: inline-block;
    width: 284px;
    height: 178px;
    text-align: center;
  }
  &__text {
    margin-top: 25px;
    font-size: 18px;
    color: #CADEFB;
    line-height: 115%;
  }
}

@media (max-width: 576px) {
  .approach {
    &__item {
      margin: 0 30px;
      height: 193px;
    }
  }
}
</style>