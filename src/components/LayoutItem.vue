<!-- MyChildComponent.vue -->
<template>
  <div>
    <div class="row">
      <div class="column">{{ item.icon }}</div>
      <div>{{ item.name }}</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "LayoutItem",
  props: {
    item: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style scoped>
/* İstediğiniz CSS stilleri */
</style>
