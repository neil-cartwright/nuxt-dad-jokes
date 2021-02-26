<template>
  <div class="container-sm">
    <AppHeader />
    <Nuxt />
  </div>
</template>
<script>
import AppHeader from "../components/AppHeader";
export default {
  components: {
    AppHeader
  }
};
</script>

<style lang="scss">
html,
.container-sm {
  padding-left: 0;
  padding-right: 0;
}
h1,
a.nav-link {
  font-family: "Single Day", display;
}
p {
  font-family: "Stylish", display;
  font-size: 1.1rem;
  color: purple;
}
h1 {
  color: yellow;
  margin-bottom: 0;
}
a.nav-link {
  color: yellow;
}
</style>
