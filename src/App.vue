<template>
  <!-- <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
  </div> -->
  <router-view />
</template>

<script src="../src/static/js/inits.js"></script>

<style>
* {
  padding: 0;
  margin: 0; 
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
  font-size: 12px;
}
input:focus-visible {
  outline: unset;
}
</style>
