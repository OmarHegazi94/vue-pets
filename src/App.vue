<template>
  <div id="app">
    <div id="nav" class="mb-5">
      <b-navbar toggleable="sm" type="light" variant="light">
        <b-navbar-toggle target="nav-text-collapse"></b-navbar-toggle>

        <b-navbar-brand>Adopt</b-navbar-brand>

        <b-collapse
          class="justify-content-center"
          id="nav-text-collapse"
          is-nav
        >
          <b-navbar-nav>
            <router-link to="/" class="mr-3">Home</router-link>
          </b-navbar-nav>

          <b-navbar-nav>
            <router-link to="/cats" class="mr-3">Cats</router-link>
          </b-navbar-nav>

          <b-navbar-nav>
            <router-link to="/dogs" class="mr-3">Dogs</router-link>
          </b-navbar-nav>
        </b-collapse>
      </b-navbar>
    </div>

    <b-container>
      <router-view />
    </b-container>
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
  // padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
