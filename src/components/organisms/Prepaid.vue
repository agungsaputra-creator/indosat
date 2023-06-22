<!-- eslint-disable vue/multi-word-component-names -->
<script setup>
import postpaid from "../../data/Postpaid";
</script>

<template>
  <div class="prepaid">
    <div class="container px-lg-5 px-3">
      <div class="row pt-5">
        <div class="col-lg-5 pt-5 d-flex justify-content-lg-end justify-content-center">
          <img
            src="../../assets/images/prepaid_person.webp"
            alt="icon postpaid"
            class="d-lg-block d-none"
          />
          <img
            src="../../assets/images/prepaid_person_mobile.webp"
            alt="icon postpaid"
            class="d-lg-none d-block"
          />
        </div>
        <div class="col-lg-7 d-flex flex-column justify-content-center">
          <h6 class="fw-bold" style="color: #898989">PREPAID</h6>
          <h3 class="fw-bold mb-xl-5 mb-4">
            Prepaid SIM Card make your days with exciting bonus and benefit
          </h3>
          <div class="row mb-xl-5 mb-md-4 mb-0">
            <div class="col-xl-4 mb-xl-0 mb-3" v-for="data in postpaid" v-bind:key="data.id">
              <MoleculeGrid v-bind:data="data" />
            </div>
          </div>
          <AtomButton class="mb-3" :link="{ name: 'Order Prepaid', url: '#' }" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import MoleculeGrid from "../molecules/MoleculeGrid.vue";
import AtomButton from "../atoms/AtomButton.vue";

export default {
  components: {
    MoleculeGrid,
    AtomButton,
  },
};
</script>

<style scoped>
.postpaid {
  background-color: #f9f9f9;
}
.postpaid-img {
  width: 30px;
}
.upgrade {
  background-color: #eeeeee;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px;
  border-radius: 8px;
}
</style>
