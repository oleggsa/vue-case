<template>
  <div class="task">
    <div class="container">
      <div class="task__content">
        <div class="header">Task</div>
        <div class="task__items">
          <TaskItem v-for="item in taskList" :key="item.id" :taskListItem="item"/>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import TaskItem from "@/components/Task/TaskItem";

export default {
  name: "index",
  data(){
    return{
      taskList: [
        {id: 1, text: 'To have all workers and their roles and responsibilities in one place',
        img: require('./../../../images/task-1.png')},
        {id: 2, text: 'To automate most of business processes and automatically track all tourists requests',
        img: require('./../../../images/task-2.png')},
        {id: 3, text: 'To automatically create a contract between tourists and agency',
        img: require('./../../../images/task-3.png')},
        {id: 4, text: 'To create a database of tourists and create instruments for their management',
        img: require('./../../../images/task-4.png')},
        {id: 5, text: 'To automatically track financing such as income, invoicing, etc',
        img: require('./../../../images/task-5.png')},
        {id: 6, text: 'To track commission of travel agents',
        img: require('./../../../images/task-6.png')},
      ]
    }
  },
  components: {
    TaskItem
  }
}
</script>

<style lang="scss" scoped>
.task {
  margin-top: 107px;
  &__items {
    margin-top: 66px;
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
  }
}
</style>