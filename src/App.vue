<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
    <router-view/>
  </div>
</template>

<style>
    @import "assets/css/peexoo.css";
    @import "assets/css/responsive.css";
    @import "assets/css/animate.css";
#app {
  font-family: 'Montserrat-Regular', Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
    margin: 0;
    padding: 0;
    color: #2c3e50;
}
</style>
