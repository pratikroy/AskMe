<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light my-navbar">
    <div class="container">
      <a class="navbar-brand">
        <router-link :to="{ name: 'home' }">AskMe</router-link>
      </a>

      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
          <li class="nav-item">
            <a class="nav-link">
              <router-link :to="{ name: 'home' }">Home</router-link>
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link">
              <router-link :to="{ name: 'about' }">About</router-link>
            </a>
          </li>
          <li class="nav-item">
            <a class="nav-link">
              <a href="/accounts/logout/" tabindex="-1">Logout</a>
            </a>
          </li>
        </ul>
        <form class="form-inline my-2 my-lg-0">
          <input class="form-control mr-sm-2" type="search" placeholder="Search" aria-label="Search">
          <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Search</button>
        </form>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "NavbarComponent"
}
</script>

<style>
  .my-navbar {
    border-bottom: 1px solid #DDD;
  }
</style>
