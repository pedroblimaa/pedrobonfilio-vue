<template>
  <div class="nav">
    <h2 class="nav-title"> <router-link to="/"> Pedro Bonfilio</router-link></h2>
    <div class="nav-options">
      <router-link to="/">About</router-link>
      <router-link to="/works">Works</router-link>
      <router-link to="/contact">Contact</router-link>
    </div>
  </div>
</template>

<script>
import './NavBar.css'

export default {
  name: "NavBar",
  props: {
    msg: String,
  },
};
</script>

