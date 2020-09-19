<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link>
      <router-link to="/about">About</router-link>
      <router-link to='/login'>Login</router-link>
      <router-link to='/user'>User</router-link>
    </div>
    <router-view/>
  </div>
</template>

<style>
  * {
    padding: 0px;
    margin: 0px;
    box-sizing:border-box;
  }

  #nav {
    display: flex;
    gap: 2em;
    margin: 2em;
    justify-content: center;
  }
</style>
