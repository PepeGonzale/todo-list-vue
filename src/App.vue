<script setup>
import { RouterLink, RouterView } from 'vue-router'
import AppHeader from '../src/components/AppHeader.vue'
import AppFooter from '../src/components/AppFooter.vue'
</script>

<template>

    <div id="app">
      <app-header></app-header>
      <RouterView class="container"></RouterView>
      <app-footer></app-footer>
    </div>

</template>
<script>

  export default {
    name: 'app',
    components: {AppHeader, AppFooter}
  }
</script>

<style scoped>
#app {
  box-sizing: border-box;
  color: #37474f;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing:antialised;
  -moz-osx-font-smoothing:grayscale;
  text-align: center;
  margin: 0 auto;
  padding: 0;
}
.container {
  padding-bottom: 4rem;
}
</style>
