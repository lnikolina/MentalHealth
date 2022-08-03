<template>
<div id="app">
  <nav id="nav" class="navbar navbar-expand-lg navbar-light bg-light">
      
        
    <a class="navbar-brand" href="#">
      <img src="@/assets/MentalHealthRGB.jpeg" 
          alt=""
          height="30" 
          class="d-inline-block align-text-top">
          MentalHealth

          <button 
            class="navbar-toggler" 
            type="button" 
            data-bs-toggle="collapse" 
            data-bs-target="#navbarSupportedContent" 
            aria-controls="navbarSupportedContent" 
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

            
          </div>

        </a>
         
  </nav>

<div class="container-fluid"></div>
<router-view/>
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

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>

