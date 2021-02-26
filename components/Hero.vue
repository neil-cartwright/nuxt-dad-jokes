<template>
  <div class="jumbotron mb-0">
    <h1 class="joke p-2 rounded" v-if="joke">{{ joke }}</h1>
    <nuxt-link to="/jokes" v-else>
      <h1 class="display-2 p-2 rounded">Dad Jokes!</h1>
    </nuxt-link>
  </div>
</template>

<script>
export default {
  props: {
    joke: {
      type: String
    }
  }
};
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

  h1,
  .joke {
    color: #fff;
    background: orange;
    opacity: 0.85;
  }
  h1.joke {
    font-size: 1.5rem;
  }
  h1 {
    font-size: 4rem;
  }
  a:hover {
    text-decoration: none;
  }
}
</style>
