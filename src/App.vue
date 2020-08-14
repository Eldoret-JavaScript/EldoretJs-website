<template>
  <div class="app">
    <Header />
    <Homepage />
    <!-- <About /> -->
  </div>
</template>

<script>
import Header from './components/Header';
import Homepage from './components/Homepage';
// import About from './components/About';
export default {
  components: {
    Header,
    Homepage,
    // About
  }
}
</script>

<style>

</style>