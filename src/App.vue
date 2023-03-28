<template>
  <div id="app">
    <!-- <IndexPage></IndexPage> -->
    <TestPage></TestPage>
  </div>
</template>

<script>
// import IndexPage from './components/IndexPage.vue';
import TestPage from './components/TestPage.vue';

export default {
  name: 'App',
  components: {
    // IndexPage
    TestPage
  }
}
</script>

<style>
* {
  padding: 0px;
  margin: 0px;
}
</style>
