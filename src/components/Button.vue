<template>
  <div>
    <button @click="onClick()" :style="{background:color}" class="btn">{{title}}</button>
  </div>
</template>

<script>
export default {
  name: 'ButtonComponent',
  props: {
    title: String,
    color: String
  },
  methods: {
    onClick() {
      console.log('clicked')
    }
  },
}
</script>

<style>
  
</style>