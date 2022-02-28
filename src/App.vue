<template>
  <div>
    <Header/>
  </div>
</template>

<script>
import Header from "@/components/Header";

export default {
  components: {Header}
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@400;500;600;700&display=swap');

* {
  box-sizing: border-box;
  font-family: 'Raleway', sans-serif;
}

body {
  background: #455db8;
  margin: 0;
  padding: 0;
}

.container {
  max-width: 940px;
  margin: 0 auto;
}
</style>
