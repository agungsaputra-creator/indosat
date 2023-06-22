<script setup>
import steps from "../../data/StepsGetCard";
</script>

<template>
  <div class="steps py-5">
    <div class="container px-lg-5 px-3">
      <AtomTitle
        tag="h3"
        content="3 easy steps to get your IM3 Ooredoo SIM Card"
        class="text-lg-center mb-lg-4 mb-3"
      />
      <AtomSubtitle
        class="text-lg-center mb-lg-5 mb-4"
        text="Now, you can easily get your IM3 Ooredoo SIM Card without hassle"
      />
      <div class="row">
        <div class="col-lg-4" v-for="data in steps" v-bind:key="data.id">
          <MoleculeGrid v-bind:data="data" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import AtomTitle from "../atoms/AtomTitle.vue";
import AtomSubtitle from "../atoms/AtomSubtitle.vue";
import MoleculeGrid from "../molecules/MoleculeGrid.vue";
export default {
  components: {
    AtomTitle,
    AtomSubtitle,
    MoleculeGrid,
  },
};
</script>

<style scoped></style>
