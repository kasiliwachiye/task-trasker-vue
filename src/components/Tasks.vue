<template>
  <div :key="task.id" v-for="task in tasks">
    <TaskComponent
      @delete-task="$emit('delete-task', task.id)"
      :task="task"
      @toggle-reminder="$emit('toggle-reminder', task.id)"
    />
  </div>
</template>
<script>
import TaskComponent from "./Task.vue";

export default {
  name: "TasksComponent",
  props: {
    tasks: Array,
  },
  components: {
    TaskComponent,
  },
  emits: ["delete-task", "toggle-reminder"],
};
</script>
<style></style>
