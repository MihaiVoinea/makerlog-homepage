<template>
  <div id="home">
    <Header />
    <main><NewTask /> <TaskList /></main>
  </div>
</template>

<script>
import Header from "../components/Header.vue";
import NewTask from "../components/NewTask.vue";
import TaskList from "../components/TasksList.vue";

export default {
  components: {
    Header,
    NewTask,
    TaskList,
  },
};
</script>

<style lang="scss" scoped>
#home {
  display: flex;
  flex-direction: column;
  align-items: center;
}
main {
  margin: 45px auto;
  width: 50%;
  min-width: 900px;
}
@media screen and (max-width: 980px) {
  main {
    min-width: 91%;
  }
}
</style>
