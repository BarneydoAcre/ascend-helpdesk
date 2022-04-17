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
input {
    border: unset;
    border-bottom: 1px solid #999;
    width: 140px;
    height: 30px;
    background: rgb(255, 255, 255,0)
}
input:focus-visible {
  outline: unset;
}
textarea {
  border: 1px solid #999;
  max-height: 100px;
  min-height: 100px;
  max-width: 100%;
  min-width: 100%;
}
textarea:focus-visible {
  outline: unset;
}
textarea:active,
textarea:hover {
  border: 1px solid #999;
}
h6 {
    margin: unset;
    padding: unset;
    font-size: 10px;
    color: #9e9e9e;
    transform: translateY(4px);
}
</style>
