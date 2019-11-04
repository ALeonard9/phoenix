<template>
  <div id="app">
    <Navbar/>
    <amplify-authenticator></amplify-authenticator>
    <Home msg="Other stuffs."/>

  </div>
</template>

<script>
import Home from './components/Home.vue'
import Navbar from './components/Navbar.vue'
// const authConfig = {
//   msg: 'You are currently signed in.', // type: string, default: null
//   signOutButton: 'Sign Out', // type: string, default: 'Sign Out', required: false
// }

export default {
  name: 'app',
  components: {
    Home,
    Navbar
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  background-color: rgba(195, 169, 240, 0.781);
}
</style>
