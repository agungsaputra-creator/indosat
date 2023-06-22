<!-- eslint-disable vue/multi-word-component-names -->

<template>
  <div class="banner">
    <div class="container px-lg-5 px-3">
      <div class="row">
        <div class="col-lg-4 order-lg-1 order-2 pt-5">
          <img src="../../assets/images/image_reminder_cta.webp" alt="banner" class="w-100" />
        </div>
        <div
          class="col-lg-8 order-lg-2 order-1 d-flex flex-column justify-content-center mt-lg-0 mt-5"
        >
          <AtomTitle
            tag="h3"
            content="Have your SIM Card delivered to vour doorster"
            class="fw-bold text-lg-start text-center mb-lg-4 mb-3"
          />
          <AtomButton class="mb-3" :link="{ name: 'Order Now', url: '#' }" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import AtomTitle from "../atoms/AtomTitle.vue";
import AtomButton from "../atoms/AtomButton.vue";

export default {
  components: {
    AtomTitle,
    AtomButton,
  },
};
</script>

<style scope>
.banner {
  background-color: #fdd401;
}
</style>
