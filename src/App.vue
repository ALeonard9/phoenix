<template>
  <div id="app">
 <b-navbar toggleable="lg" type="dark" variant="dark" fixed="top">
    <b-navbar-brand href="#">
      Adam Leonard
    </b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item href="#" disabled>Books</b-nav-item>
        <b-nav-item href="#">Countries</b-nav-item>
        <b-nav-item href="#" disabled>Movies</b-nav-item>
        <b-nav-item href="#" disabled>TV</b-nav-item>
        <b-nav-item href="#" disabled>Video Games</b-nav-item>
      </b-navbar-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">

        <b-nav-item-dropdown right>
          <!-- Using 'button-content' slot -->
          <template v-slot:button-content>
            <em>User</em>
          </template>
          <b-dropdown-item href="#">Profile</b-dropdown-item>
          <b-dropdown-item href="#">Sign Out</b-dropdown-item>
        </b-nav-item-dropdown>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>

    <HelloWorld msg="Vue stuffs."/>
    <a target="_blank" href="https://www.linkedin.com/in/aleonard9/">
      <img class="logo" src="@/assets/linkedin_logo.svg" title="Linkedin">
    </a>
    <a target="_blank" href="https://github.com/ALeonard9">
      <img class="logo" src="@/assets/github_logo.svg" title="Github Account">
    </a>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'app',
  components: {
    HelloWorld
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
}
.logo{
  height:12%;
  width:12%;
  margin: 10%;
  margin-top: 15%;
}
</style>
