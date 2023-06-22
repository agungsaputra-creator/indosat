<template>
  <component :is="tag">{{ content }}</component>
</template>

<script>
export default {
  name: "AtomTitle",
  props: ["tag", "content"],
};
</script>
