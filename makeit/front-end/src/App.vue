<template>
  <div id="app">
     <b-navbar toggleable="lg" type="dark" variant="info">
    

    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item to= "/" >Home</b-nav-item>
        <b-nav-item href="/about" >Create</b-nav-item>

        <b-nav-item-dropdown text="Categories" right>
          <b-dropdown-item href="#">Games</b-dropdown-item>
          <b-dropdown-item href="#">Anime</b-dropdown-item>
          <b-dropdown-item href="#">Series</b-dropdown-item>
          <b-dropdown-item href="#">Movies</b-dropdown-item>
        </b-nav-item-dropdown>
      </b-navbar-nav>
<!--Center -->
<div>
<b-navbar-brand class="title" href="#">What have you watched?</b-navbar-brand>
</div>
      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-form>
          <b-form-input size="sm" class="mr-sm-2" placeholder="Search"></b-form-input>
          <b-button size="sm" class="my-2 my-sm-0" type="submit">Search</b-button>
        </b-nav-form>

      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
    <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view/>
    
  </div>
  
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
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
