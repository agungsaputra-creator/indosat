<!-- eslint-disable vue/multi-word-component-names -->

<script setup>
import activity from "../../data/Activity";
</script>

<template>
  <div class="activity py-5">
    <div class="container px-lg-5 px-3">
      <AtomTitle
        tag="h3"
        content="Already place on order for IM3 Ooredoo SIM Card?"
        class="fw-bold text-center mb-xl-5 mb-4"
      />
      <div class="row">
        <div class="col-lg-6 mb-lg-0 mb-3" v-for="data in activity" v-bind:key="data.id">
          <MoleculeCard v-bind:data="data" />
        </div>
        <div class="col-lg-6 mb-lg-0 mb-3"></div>
      </div>
    </div>
  </div>
</template>

<script>
import AtomTitle from "../atoms/AtomTitle.vue";
import MoleculeCard from "../molecules/MoleculeCard.vue";

export default {
  AtomTitle,
  MoleculeCard,
};
</script>

<style scoped>
.activity {
  background-color: #f9f9f9;
}
</style>
