<template>
  <div class="card mt-2">
    <div class="card-body bg-light">
      <form action="" @submit.prevent="onSubmit">
        <div class="row">
          <div class="col">
            <input
              type="text"
              class="input form-control"
              v-model="text"
              placeholder="search jokes"
              autofocus
            />
          </div>
          <div class="col">
            <input type="submit" class="btn btn-success" value="search" />
          </div>
        </div>
      </form>
    </div>
  </div>
</template>
<style scoped></style>
<script>
export default {
  name: "SearchJokes",
  data() {
    return {
      text: ""
    };
  },
  methods: {
    onSubmit: function() {
      this.$emit("search-text", this.text);
      this.$text = "";
    }
  }
};
</script>
