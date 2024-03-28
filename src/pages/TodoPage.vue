<!-- MyParentComponent.vue -->
<template>
  <div>
    <div v-for="(item, index) in tasks" :key="index">
      <Todo :todo="item" />
    </div>
  </div>
</template>

<script>
import Todo from "components/Todo.vue";

export default {
  name: "TodoPage",
  components: {
    Todo,
  },
  data() {
    return {
      tasks: [
        { id: 1, task: "Vue.js öğrenmek", responsible: "Ahmet" },
        { id: 2, task: "React uygulaması geliştirmek", responsible: "Ayşe" },
        { id: 3, task: "Angular projesi tasarlamak", responsible: "Mehmet" },
      ],
    };
  },
};
</script>

<style scoped>
/* İstediğiniz CSS stilleri */
</style>
