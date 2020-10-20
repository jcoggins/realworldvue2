<template>
  <div id="app">
    <div id="nav">
      <!--
      <router-link to="/">Show Listing</router-link> |
      <router-link to="/event">Show Event #1</router-link> |
      <router-link to="/event/create">Create</router-link> |
      -->
      <!--  It works !! -->
      <router-link :to="{ name: 'event-list' }">List</router-link> |
      <router-link :to="{ name: 'event-create' }">Create</router-link>
    </div>
    <router-view />
  </div>
</template>

<style>
  #app {
    font-family: 'Avenir', Arial, Helvetica, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50
  }
  #nav {
    padding: 30px;
  }

  #nav a {
  font-weight: bold;
  color: #2c3e50;
  }

  #nav a.router-link-exact-active {
  color: #42b983;
  }
</style>