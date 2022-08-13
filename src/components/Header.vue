<template>
  <div>
    <header>
      <h1>{{ title }}</h1>
      <ButtonComponent title="Add Task" color="green" />
    </header>
  </div>
</template>

<script>
import ButtonComponent from "./Button.vue";

export default {
  name: "HeaderComponent",
  props: {
    title: {
      type: String,
    },
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
