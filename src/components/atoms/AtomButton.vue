<!-- eslint-disable vue/multi-word-component-names -->

<template>
  <a :href="link.url" class="btn-indosat text-decoration-none">
    {{ link.name }}
  </a>
</template>

<script>
export default {
  name: "AtomButton",
  props: ["link"],
};
</script>

<style scoped></style>
