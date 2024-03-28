<!-- MyChildComponent.vue -->
<template>
  <div class="q-pa-md example-column-flex-order">
    <div class="row">
      <div class="column">{{ todo.id }}</div>
      <div class="column">
        <div>{{ todo.task }}</div>
        <div>{{ todo.responsible }}</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Todo",
  props: {
    todo: {
      type: Object,
      required: true,
    },
  },
};
</script>

<style scoped>
/* İstediğiniz CSS stilleri */
</style>
