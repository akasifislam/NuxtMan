<template>
  <div class="">
    <h1>sub id sub id: {{ $route.params.id }}</h1>
  </div>
</template>

<script>
export default {
  validate({params}) {
    return /^\d+$/.test(params.id);
  },
};
</script>

<style>
</style>