<!-- eslint-disable vue/multi-word-component-names -->
<script setup>
import postpaid from "../../data/Postpaid";
</script>

<template>
  <div class="postpaid">
    <div class="container px-lg-5 px-3">
      <div class="row">
        <div
          class="col-lg-7 order-lg-1 order-2 pb-lg-0 pb-5 d-flex flex-column justify-content-center"
        >
          <h6 style="color: #898989" class="fw-bold">POSTPAID</h6>
          <h3 class="fw-bold mb-xl-5 mb-4">
            Free yourself from reload routine, Subscribe <span class="font-primary">Prime</span> &
            <span class="font-primary">get bill discount up to 300k</span>
          </h3>
          <div class="row mb-xl-5 mb-md-4 mb-0">
            <div class="col-xl-4 mb-xl-0 mb-3" v-for="data in postpaid" v-bind:key="data.id">
              <MoleculeGrid v-bind:data="data" />
            </div>
          </div>
          <AtomButton class="mb-4" :link="{ name: 'subscribe postpaid', url: '#' }" />
          <div class="upgrade">
            <AtomSubtitle
              class="fw-bold mb-sm-0 mb-1"
              text="Already have prepaid number? Upgrade to postpaid"
            />
            <a href="" class="text-decoration-none fw-bold font-primary">Upgrade now</a>
          </div>
        </div>
        <div class="col-lg-5 order-lg-1 order-1 pt-5 d-flex justify-content-center">
          <img
            src="../../assets/images/postpaid_person.webp"
            alt="icon postpaid"
            class="d-lg-block d-none"
          />
          <img
            src="../../assets/images/postpaid_person_mobile.webp"
            alt="icon postpaid"
            class="d-lg-none d-block"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import MoleculeGrid from "../molecules/MoleculeGrid.vue";
import AtomButton from "../atoms/AtomButton.vue";
import AtomSubtitle from "../atoms/AtomSubtitle.vue";

export default {
  components: {
    MoleculeGrid,
    AtomButton,
    AtomSubtitle,
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
@media only screen and (max-width: 992px) {
  .upgrade {
    display: flex;
    flex-direction: column;
  }
}
@media only screen and (max-width: 576px) {
  .upgrade {
    align-items: flex-start;
  }
}
</style>
