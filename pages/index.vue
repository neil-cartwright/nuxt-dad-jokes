<template>
  <div>
    <Hero />
  </div>
</template>

<script>
import Hero from "~/components/Hero";
export default {
  components: {
    Hero
  },
  head() {
    return {
      title: "Welcome to dad jokes",
      meta: [
        {
          hid: "description",
          name: "description",
          content: "Best place for corny dad jokes"
        }
      ]
    };
  }
};
</script>

<style lang="scss"></style>
