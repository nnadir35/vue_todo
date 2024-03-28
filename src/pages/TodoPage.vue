<!-- MyParentComponent.vue -->
<template>
  <q-page>
    <div>
      <div v-for="(item, index) in tasks" :key="index">
        <Todo :todo="item" />
      </div>
    </div>
  </q-page>
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
        { id: 1, task: "Vue.js öğrenmek", completed: false },
        { id: 2, task: "React uygulaması geliştirmek", completed: false },
        { id: 3, task: "Angular projesi tasarlamak", completed: false },
      ],
    };
  },
};
</script>

<style scoped>
/* İstediğiniz CSS stilleri */
</style>
