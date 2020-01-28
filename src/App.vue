<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">Home</router-link> 
      <router-link to="/about">About</router-link> 
      <router-link to="/services">Services</router-link> 
    </div>
    <router-view/>
  </div>
</template>

<style>

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
 background-color: rgba(0, 0, 0, 0.658);
  text-align: center;
  color: white;
}

#nav {
  padding: 30px;
  background-color: #42b983;
  margin-bottom: 20px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
  text-decoration: none;
  padding:0px 20px
}

#nav a.router-link-exact-active {
  border-bottom: 1px solid #2c3e50;
  color:black;
}

</style>
