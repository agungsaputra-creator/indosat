<!-- eslint-disable vue/multi-word-component-names -->

<template>
  <div class="footer py-5">
    <div class="container">
      <div class="row d-flex justify-content-center">
        <div class="col-xl-6 col-md-12">
          <div class="row">
            <div class="col-md-4 col-12 mb-md-0 mb-3 border-right">
              <AtomSubtitle class="text-white fw-bold mb-2" text="Support" />
              <AtomSubtitle class="text-white-50 mb-2" text="Promotion" />
              <AtomSubtitle class="text-white-50 mb-2" text="FAQ" />
              <AtomSubtitle class="text-white-50 mb-2" text="Terms & Conditions" />
              <AtomSubtitle class="text-white-50 mb-2" text="Privacy Policy" />
              <AtomSubtitle class="text-white-50 mb-2" text="Coverage Map" />
            </div>
            <div class="col-md-4 col-12 mb-md-0 mb-3 border-right">
              <AtomSubtitle class="text-white fw-bold mb-2" text="Investor Relations" />
              <AtomSubtitle class="text-white-50 mb-2" text="About Indosat Ooredoo" />
              <AtomSubtitle class="text-white-50 mb-2" text="Ideabox" />
              <AtomSubtitle class="text-white-50 mb-2" text="Press Release" />
              <AtomSubtitle class="text-white-50 mb-2" text="Careers" />
            </div>
            <div class="col-md-4 col-12 mb-md-0 mb-3">
              <AtomSubtitle class="text-white fw-bold mb-2" text="Kontak Kami" />
              <AtomSubtitle class="text-white-50 mb-2" text="Contact Information" />
              <AtomSubtitle class="text-white-50 mb-2" text="Find a Store" />
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import AtomSubtitle from "../atoms/AtomSubtitle.vue";

export default {
  components: {
    AtomSubtitle,
  },
};
</script>

<style scoped>
.footer {
  background-color: #000;
}
</style>
