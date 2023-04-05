<template>
<div class="app">
  <nav id = "nav" class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">
      <img src="@/assets/fipu_logo.png" height="40" class="d-inline-block align-top" alt="" loading="lazy"/>
    </a>
    <button 
      class="navbar-toggler" 
      type="button" 
      data-bs-toggle="collapse" 
      data-bs-target="#navbarSupportedContent" 
      aria-controls="navbarSupportedContent" 
      aria-expanded="false" 
      aria-label="Toggle navigation"
      >
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item">
          <router-link to="/" class="nav-link">Home</router-link>
        </li>
        <li class="nav-item">
          <router-link to="/login" class="nav-link">Login</router-link>
        </li>
        <li class="nav-item">
          <router-link to="/signup" class="nav-link">Sign up</router-link>
        </li>
      </ul>
      <form class="d-flex" role="search">
        <input class="form-control me-2" type="search" placeholder="Pretraga" aria-label="Search">
        
      </form>
    </div>
  </div>
</nav>
</div>

<div class="container">
  <router-view />
</div>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
  background-color: white !important;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>

<!-- <router-link to="/" class="nav-link">Home</router-link>
<router-link to="/login" class="nav-link">Login</router-link>
<router-link to="/signup" class="nav-link">Sign up</router-link>

<template>
  <div id = "app">
    <nav id = "nav" class = "navbar navbar-light bg-light">
    <a class="navbar-brand" href="#">
      <img src="@/assets/fipu_logo.png" height="40" class="d-inline-block align-top" alt="" loading="lazy"/>
    </a> -->