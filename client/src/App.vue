<template>
  <div class="app">
    <Nav/>
    <router-view/>
  </div>
</template>

<script>
import  Nav from './components/Nav.vue'
export default {
  components: {
    Nav
  }
}
</script>

<style>
.app {
  overflow: hidden;
  width: 100%;
}
</style>