<template>
<div id="app">
  <nav id="nav" class="navbar navbar-expand-lg navbar-light bg-light">
    <a class="navbar-brand" href="#">
      <img src="@/assets/MentalHealthRGB.jpeg" 
          class="d-inline-block align-top"
          alt=""
          height="30" 
          loading="lazy" />
          MentalHealth
    </a>      

          <button 
            class="navbar-toggler" 
            type="button" 
            data-toggle="collapse" 
            data-target="#navbarToggler" 
            aria-controls="navbarToggler" 
            aria-expanded="false" 
            aria-label="Toggle navigation">

            <span class="navbar-toggler-icon"></span>
          </button>
 
          <div class="collapse navbar-collapse" id="navbarToggler">
              <ul class="navbar-nav mr-auto mt-2 mt-lg-0">
                  <li class="nav-item">
                    <router-link to="/" class="nav-link">Home</router-link>
                  </li>
                  <li class="nav-item">
                    <router-link to="/login" class="nav-link">Login</router-link>
                  </li>
                  <li class="nav-item">
                    <router-link to="/singup" class="nav-link">Singup</router-link>
                  </li>
              </ul>  
              
              
      <form class="d-flex" role="search">
        <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
      </form>

          </div>  
          
              
  </nav>
   

  <div class="container">
    <router-view/>
  </div>
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

nav {
  padding: 30px;
  background-color: #81CBC7;
  color: #81CBC7;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>

