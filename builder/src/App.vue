<template>
  <TheHead h1="РЕАЛИЗУЕМ КРУПНЕЙШИЕ
  ПРОЕКТЫ В РОССИИ" 
  p="стадионы, газопроводы, мосты, дамбы"></TheHead>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import TheHead from './components/TheHead.vue';

export default defineComponent({
  name: 'App',
  components: {
    TheHead
  }
});
</script>

<style>
* {
  margin: 0;
  padding: 0;
}
#app {
  
}
</style>
