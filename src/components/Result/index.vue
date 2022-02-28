<template>
  <div class="result">
    <div class="container">
      <div class="result__content">
        <div class="header">Result</div>
        <div class="result__text">CRM works as a web application. The applications streamlines
          and automates most of the processes, helps track financial information and safely keeps
          client information for future use.</div>
        <img src="./../../../images/result.png" alt="result">
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
.result {
  &__content {
    margin-top: 90px;
    & img {
      margin-top: 30px;
    }
  }
  &__text {
    margin-top: 87px;
    font-size: 24px;
    color: #CADEFB;
    text-align: center;
  }
}
</style>