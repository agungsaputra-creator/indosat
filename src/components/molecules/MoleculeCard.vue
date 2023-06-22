<!-- eslint-disable vue/multi-word-component-names -->

<template>
  <div class="card card-indosat">
    <div class="card-body">
      <div class="d-flex align-items-center">
        <img :src="data.image" alt="icon postpaid" />
        <div class="ms-4">
          <h4 class="mb-3">{{ data.title }}</h4>
          <p class="font-dark mb-3 fw-lighter">{{ data.subtitle }}</p>
          <a href="" class="text-decoration-none fw-bold" style="color: #ed2324">
            {{ data.link }}
          </a>
        </div>
      </div>
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
.card-indosat {
  padding: 20px 10px;
  border-radius: 16px;
  box-shadow: 0 10px 10px 0 rgba(0, 0, 0, 0.1);
  border: none;
}
</style>
