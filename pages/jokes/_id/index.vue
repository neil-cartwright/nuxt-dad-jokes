<template>
  <div>
    <Hero />
    <div class="card mt-2">
      <div class="card-body">
        {{ joke }}
      </div>
    </div>
    <hr />
    <small>Joke ID: {{ $route.params.id }}</small>
  </div>
</template>
<script>
import axios from "axios";
import Hero from "~/components/Hero";
export default {
  components: {
    Jumbotron
  },
  data() {
    return {
      joke: {}
    };
  },
  async created() {
    const config = {
      headers: {
        Accept: "application/json"
      }
    };
    try {
      const res = await axios.get(
        `https://icanhazdadjoke.com/j/${this.$route.params.id}`,
        config
      );
      this.joke = res.data.joke;
    } catch (err) {
      console.log(err);
    }
  }
};
</script>
