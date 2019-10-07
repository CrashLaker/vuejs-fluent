<template>
    <div id="app">
        <Navbar />
        <!--<nav>
      <div class="nav-wrapper">
        <a href="#" class="brand-logo">Capacity Planning</a>
        <ul id="nav-mobile" class="right hide-on-med-and-down">
          <li><router-link to="/">Home</router-link></li>
          <li><router-link to="/about">About</router-link></li>
          <li><router-link to="/icons">Icons</router-link></li>
        </ul>
      </div>
    </nav>
    <div id="nav">
        </div>-->
        <router-view />
    </div>
</template>

<script>
import Navbar from "@/views/Navbar.vue";

export default {
    components: {
        Navbar
    }
};
</script>

<style>
</style>
