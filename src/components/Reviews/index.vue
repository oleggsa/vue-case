<template>
  <div class="reviews">
    <div class="container">
      <div class="reviews__content">
        <div class="header">Reviews</div>
        <img src="./../../../images/reviews.png" alt="reviews">
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
.reviews {
  margin-top: 104px;
  margin-bottom: 200px;
  &__content {
    text-align: center;
    & img {
      margin-top: 89px;
    }
  }
}
</style>