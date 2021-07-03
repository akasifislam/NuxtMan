<template>
  <div class="container">
    <h1>Nested User Page</h1>

    <input type="text" v-model="id" />
    <button @click="loadUser">Load User</button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      id: "",
    };
  },
  methods: {
    loadUser() {
      this.$router.push(`/user/${this.id}`);
    },
  },
};
</script>

<style>
</style>