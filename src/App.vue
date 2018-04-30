<template>
  <div id="app">
    <div class="bs-component">
              <nav class="navbar navbar-expand-lg navbar-dark bg-primary">
                <a class="navbar-brand" href="#">Flapjack</a>
                <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarColor01" aria-controls="navbarColor01" aria-expanded="false" aria-label="Toggle navigation">
                  <span class="navbar-toggler-icon"></span>
                </button>

                <div class="collapse navbar-collapse" id="navbarColor01">
                  <ul class="navbar-nav mr-auto">
                    <li class="nav-item active">
                      <a class="nav-link"><router-link to="/"  class="nav-link" exact>Home</router-link> <span class="sr-only">(current)</span></a>
                    </li>
                    <li class="nav-item">
                      <a class="nav-link"><router-link to="/topics"  class="nav-link">Topics</router-link></a>
                    </li>
                    <li class="nav-item">
                      <a class="nav-link"><router-link to="/counter"  class="nav-link">Counter</router-link></a>
                    </li>
                    <li class="nav-item">
                      <a  class="nav-link" ><router-link to="/about" class="nav-link">About</router-link></a>
                    </li>
                  </ul>
                  <form class="form-inline my-2 my-lg-0">
                    <input class="form-control mr-sm-2" type="text" placeholder="Search">
                    <button class="btn btn-secondary my-2 my-sm-0" type="submit">Search</button>
                  </form>
                </div>
              </nav>
            </div>
    <div class="container">
      <router-view class="view"></router-view>
    </div>
  </div>
</template>

<style>
body {
  font-family: Helvetica, sans-serif;
}
.router-link {
  color: rgba(255, 255, 255, 0.5);
}
.router-link-active {
  color: white;
}
</style>
