<script setup lang="ts">
import AppHeader from './components/AppHeader.vue';
import TodoList from './components/TodoList.vue';
</script>

<template>
  <div class="content-wrap">
    <AppHeader />
    <TodoList />
  </div>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

.content-wrap{
  display: flex;
  flex-direction: column;
}

@media (min-width: 1024px) {
  header {
    display: block;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
