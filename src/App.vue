<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> 
       <router-link to="/login">Login</router-link> 
       <router-link to="/signin">Sign in</router-link>
      <router-link to="/about">About</router-link>
    </div>
    <router-view/>
  </div>
</template>

<style lang="less">
*{
    margin: 0;
    padding: 0;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
    width: 80%;
    height: 50px;
    margin: 0 auto;
    display: flex;
    justify-content: flex-end;
  a {
      list-style: none;
      text-decoration-line: none;
    font-weight: bold;
    color: #2c3e50;
    margin-right: 20px;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
