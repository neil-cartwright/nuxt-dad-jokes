<template>
  <nuxt-link :to="'jokes/' + id">
    <div class="joke card my-2">
      <div class="card-body">
        <p>{{ joke }}</p>
      </div>
    </div>
  </nuxt-link>
</template>
<script>
export default {
  name: "Joke",
  props: ["joke", "id"]
};
</script>

<style lang="scss">
.card.joke {
  display: flex;
  align-items: center;

  &:hover {
    background: ghostwhite;
  }
}
p {
  margin-bottom: 0;
}
a {
  color: black;

  &:hover {
    color: black;
    opacity: 0.9;
  }
}
</style>
