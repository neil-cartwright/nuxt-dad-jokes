<template>
  <nav class="navbar navbar-light bg-primary navbar-expand-lg py-2">
    <div class="container">
      <nuxt-link to="/" class="navbar-brand">
        <h1>Dad Jokes</h1>
      </nuxt-link>
    </div>
    <ul class="navbar-nav my-2, my-lg-0, me-sm-0, my-sm-0">
      <nuxt-link to="/jokes" class="nav-link">Jokes</nuxt-link>
    </ul>
  </nav>
</template>
<script>
export default {
  name: "AppHeader"
};
</script>
<style>
.nav-link {
  color: yellow !important;
  font-size: 1.2rem;
}
</style>
