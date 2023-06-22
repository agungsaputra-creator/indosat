<!-- eslint-disable vue/multi-word-component-names -->

<template>
  <div class="sosmed">
    <AtomTitle tag="h5" content="Social Media" class="text-center text-light mb-2" />
  </div>
</template>

<script>
import AtomTitle from "../atoms/AtomTitle.vue";

export default {
  components: {
    AtomTitle,
  },
};
</script>

<style scoped>
.sosmed {
  padding: 30px 0;
  background-color: #ed2324;
}
</style>
