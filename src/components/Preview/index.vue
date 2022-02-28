<template>
  <div class="preview">
    <div class="container">
      <div class="preview__text">
        <div class="preview__text title">
          Customer relations management application
        </div>
        <div class="preview__text subtitle">
          Love to travel CRM
        </div>
        <div class="preview__text desqr">
          The goal of the application is to have a CRM fully customized for internal purposes.<br>
          Application has a streamline process which optimizes the process of working with tourists,
          helps to track statistics, automates most of the processes and automatically adds accounting
          records and exports accounting reports.
        </div>
        <div class="preview__text-img">
          <img src="../../../images/top-screenshot.png" alt="screenshot">
        </div>
        <div class="preview__image"><img src="../../../images/top-screen.png" alt="screen"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header"
}
</script>

<style lang="scss" scoped>
$color: red;

.preview {
  overflow-x: hidden;
  margin-top: 58px;
  &__text {
    width: 500px;
    display: inline-block;
    position: relative;
    & .title {
      color: white;
      font-weight: bold;
      font-size: 70px;
    }
    & .subtitle {
      color: #3B9DE8;
      font-weight: bold;
      font-size: 70px;
      margin-top: 10px;
    }
    & .desqr {
      color: white;
      font-weight: 600;
      font-size: 18px;
      margin-top: 20px;
    }
    &-img {
      margin-top: 18px;
    }
  }
  &__image {
    display: inline-block;
    position: absolute;
    top: 134px;
    left: 584px;
  }
}
</style>