<!-- eslint-disable vue/multi-word-component-names -->

<template>
  <div class="d-flex justify-content-center align-items-center mb-lg-0 mb-4">
    <div class="flex-shrink-0">
      <img :src="data.image" alt="icon sim card" class="step-img" />
    </div>
    <div class="flex-grow-1 ms-4">
      <p class="fw-bold mb-1">{{ data.title }}</p>
      <p class="step-text font-dark text-break mb-0">{{ data.subtitle }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "MolekulGrid",
  props: ["data"],
};
</script>

<style scoped>
.step-img {
  width: 40px;
}
.step-text {
  width: 80%;
  font-weight: 300;
}
@media only screen and (max-width: 992px) {
  .step-text {
    width: 100%;
  }
}
</style>
