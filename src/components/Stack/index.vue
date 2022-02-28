<template>
  <div class="stack">
    <div class="container">
      <div class="stack__content">
        <div class="header">Technology Stack</div>
        <div class="stack__first-row">
          <img src="./../../../images/stack-1.png" alt="stack1">
          <img src="./../../../images/stack-2.png" alt="stack2">
          <img src="./../../../images/stack-3.png" alt="stack3">
        </div>
        <div class="stack__second-row">
          <img src="./../../../images/stack-4.png" alt="stack4">
          <img src="./../../../images/stack-5.png" alt="stack5">
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
    }
   }
  &__first-row {
    margin-top: 95px;
  }
  &__second-row {
    margin-top: 46px;
  }
}
</style>