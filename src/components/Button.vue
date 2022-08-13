<template>
  <div>
    <button
      @click="$emit('btn-click')"
      :style="{ background: color }"
      class="btn"
    >
      {{ title }}
    </button>
  </div>
</template>

<script>
export default {
  name: "ButtonComponent",
  props: {
    title: String,
    color: String,
  },
};
</script>

<style></style>
