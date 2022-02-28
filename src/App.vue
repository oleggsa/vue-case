<template>
  <div>
    <Preview/>
    <Task/>
    <Stack/>
    <Approach/>
  </div>
</template>

<script>
import Preview from "@/components/Preview";
import Task from "@/components/Task";
import Stack from "@/components/Stack";
import Approach from "@/components/Approach";

export default {
  components: {
    Preview,
    Task,
    Stack,
    Approach
  }
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@400;500;600;700&family=Roboto:wght@700&display=swap');

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

.header {
  font-weight: bold;
  font-size: 70px;
  color: #CADEFB;
  text-transform: uppercase;
  text-align: center;
}
</style>
