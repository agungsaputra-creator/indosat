<!-- eslint-disable vue/multi-word-component-names -->

<template>
  <div class="pt-4">
    <AtomButton class="text-danger" :link="{ name: 'ButtonTest', url: '#' }" />
  </div>
</template>

<script>
import AtomButton from "../atoms/AtomButton.vue";

export default {
  name: "MolekulBanner",
  components: {
    AtomButton,
  },
};
</script>

<style scoped></style>
