<template>
  <div>
    <header>
      <h1>{{ title }}</h1>
      <ButtonComponent
        :title="showAddTask ? 'Close' : 'Add Task'"
        :color="showAddTask ? 'red' : 'green'"
        @btn-click="$emit('toggle-add-task')"
      />
    </header>
  </div>
</template>

<script>
import ButtonComponent from "./Button.vue";

export default {
  name: "HeaderComponent",
  props: {
    title: String,
    showAddTask: Boolean,
  },
  components: {
    ButtonComponent,
  },
};
</script>

<style>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>
