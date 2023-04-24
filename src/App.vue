<template>
<div id="app">
<!-- <img alt="Vue logo" src="./assets/logo.png"> -->
<HomePage/>
<AdminPage/>
</div>

</template>

<script>
import AdminPage from './components/admin.vue';
import HomePage from './components/Home.vue'
export default {
  name: 'App',
  components: {
    HomePage,
    AdminPage,
  }
}
</script>

<style>
#app {
  margin-top:0;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
