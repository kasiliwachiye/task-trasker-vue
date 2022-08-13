<template>
  <footer>
    <p>Copyright &copy; {{year}}</p>
    <router-link to="/about">About</router-link>
  </footer>
</template>

<script>
export default {
  name: "FooterComponent",
  data() {
    return {
      year: new Date().getFullYear(),
    };
  },
};
</script>

<style scoped>
a {
  color: #333;
}

footer {
  margin-top: 30px;
  text-align: center;
}
</style>