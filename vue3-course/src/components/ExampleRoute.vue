<!-- Structure extracted from the website: https://vuejs.org/guide/scaling-up/routing.html -->

<!-- SCRIPT -->
<script setup>
  // Imports of Vue
  import { ref, computed } from 'vue'

  // Pages
  import Page1 from './PageOne.vue'
  import Page2 from './PageTwo.vue'
  import PageError from './PageError.vue'

  // Create one struct of route, containing the path and component
  const routes = {
    '/': Page1,
    '/page2': Page2,
    '/404': PageError
  }

  // Get the content from cerquila, example: http://localhost:5173/#/about the return will be: #/about
  const refRoute = ref(window.location.hash)

  // Executes the action when navigating between pages. Get content from hash
  window.addEventListener('hashchange', () => {
    refRoute.value = window.location.hash
  });

  // Function responsible for displaying the specific page
  const currentView = computed(() => {
    return routes[refRoute.value.slice(1) || '/'] || PageError
  })
</script>

<!-- TEMPLATE -->
<template>
  <!-- Links -->
  <a href="#/">Page 1</a>
  |
  <a href="#/page2">Page 2</a>

  <!-- Page display -->
  <component :is="currentView" />
</template>