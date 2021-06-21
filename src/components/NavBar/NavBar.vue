<template>
  <div v-bind:class="{ 'transparent': isHome }" class="nav">
    <h2 class="nav-title"><router-link to="/"> Pedro Bonfilio</router-link></h2>
    <div class="nav-options">
      <router-link v-on:click.native="isHome = true" to="/">About</router-link>
      <router-link v-on:click.native="isHome = false" to="/works">
        Works
      </router-link>
      <router-link v-on:click.native="isHome = false" to="/contact">
        Contact
      </router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "NavBar",
  data: function () {
    return {
      isHome: this.navTransparent,
    };
  },
  props: {
    navTransparent: {
      default: false,
    },
  },
  mounted: function (){
    this.isHome = window.location.href.split('/')[3] ? false : true;
  },
};
</script>

<style scoped src="./NavBar.css">
</style>

