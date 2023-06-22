<!-- eslint-disable vue/multi-word-component-names -->

<template>
  <div class="terms">
    <AtomTitle tag="h6" content="Terms & Conditions" class="text-center text-light mb-2" />
    <AtomSubtitle class="pxsmall text-center text-light" text="Read All" />
  </div>
</template>

<script>
import AtomTitle from "../atoms/AtomTitle.vue";
import AtomSubtitle from "../atoms/AtomSubtitle.vue";

export default {
  components: {
    AtomTitle,
    AtomSubtitle,
  },
};
</script>

<style scoped>
.terms {
  padding: 30px 0;
  background-color: #a2a1a1;
  border-radius: 8px;
}
</style>
