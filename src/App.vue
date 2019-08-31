<template>
  <div id="app">
    <div class="row no-gutters vh-100">
      <div class="col-2 bg-secondary text-light d-none d-md-block sidebar">
        <div class="sticky-top">
          <nav id="nav" class="navbar navbar-expand navbar-dark py-4 sticky-top d-flex justify-content-center">
            <router-link to="/" class="navbar-brand">
              <img class="img-fluid" src="/img/logo-white.png" alt="">
            </router-link>
          </nav>
          <ul class="nav flex-column">
            <li class="nav-item">
              <router-link to="/" class="nav-link text-light">Home</router-link>
            </li>
            <li class="nav-item">
              <router-link to="/about" class="nav-link text-light">About</router-link>
            </li>
          </ul>
        </div>
      </div>
      <div class="col bg-light d-flex flex-column">
        <nav id="nav" class="navbar navbar-expand navbar-light bg-white d-flex shadow-sm py-4 sticky-top">
          <router-link to="/" class="navbar-brand d-none d-md-block">Company Name</router-link>
          <form class="form-inline mr-auto flex-fill d-flex">
              <input class="form-control mr-sm-3 flex-fill shadow-sm border-0" type="search" placeholder="Search" aria-label="Search">
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
        <div class="px-5 pt-5 flex-fill" style="overflow-y:scroll">
          <router-view/>
        </div>
      </div>
    </div>
  </div>
</template>
