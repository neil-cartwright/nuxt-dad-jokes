<template>
  <div class="jumbotron mb-0">
    <nuxt-link to="/jokes">
      <h1 class="display-2 p-2 rounded">Dad Jokes!</h1>
    </nuxt-link>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.jumbotron {
  background: url("~assets/images/dad-jokes-processed.jpg");
  background-size: cover;
  background-position: center;
  min-height: calc(100vh - 80px);
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 0;

  h1 {
    color: #fff;
    background: orange;
    opacity: 0.85;
  }
  a:hover {
    text-decoration: none;
  }
}
</style>
