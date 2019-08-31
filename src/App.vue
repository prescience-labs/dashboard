<template>
  <div id="app" class="vh-100 d-flex flex-column">
    <div class="row sticky-top">
      <div class="col">
        <nav id="nav" class="navbar navbar-expand navbar-dark bg-secondary d-flex shadow-sm py-4">
          <router-link to="/" class="navbar-brand">
            <img class="img-fluid" src="/img/logo-white.png" alt="">
          </router-link>
          <form class="form-inline ml-3 mr-auto flex-fill d-flex">
              <input class="form-control form-control-lg mr-sm-3 flex-fill shadow-sm border-0" type="search" placeholder="Search" aria-label="Search">
          </form>
          <ul class="navbar-nav">
            <li class="nav-item">
              <router-link to="/about" class="nav-link">About</router-link>
            </li>
            <li class="nav-item dropdown">
              <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                User Name
              </a>
              <div class="dropdown-menu dropdown-menu-right border-0 shadow" aria-labelledby="navbarDropdown">
                <a class="dropdown-item" href="#">Account</a>
                <a class="dropdown-item" href="#">Sign out</a>
              </div>
            </li>
          </ul>
        </nav>
      </div>
    </div>

    <div class="row flex-fill">
      <div class="col bg-light d-flex flex-column">
        <div class="pt-5 flex-fill" style="overflow-y:scroll">
          <router-view/>
        </div>
      </div>
    </div>

    <footer class="text-muted bg-light py-5">
      <div class="container text-center">
        Made with &lt;3 in Utah.
      </div>
    </footer>
  </div>
</template>
