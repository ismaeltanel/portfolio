<!-- components/Navbar.vue -->

<template>
  <div class="container">
    <nav class="navbar" role="navigation" aria-label="main navigation">
      <div class="navbar-brand">
        <a class="navbar-item" href="/"><img src="~/assets/Logo.png" /></a>
        <!--<button class="button navbar-burger">
          <span></span>
          <span></span>
          <span></span>
        </button>-->
      </div>
      <div class="navbar-menu">
        <div class="navbar-end">
          <!--<a class="navbar-item" href="#about">About</a>
          <a class="navbar-item" href="#works">Works</a>
          <a class="navbar-item" href="#contact">Contact</a>-->
        </div>
      </div>
    </nav>
  </div>
</template>

<style scoped>

.container {
    position: fixed;
    left: 0;
    right: 0;
    top: 2vh;
    z-index: 999;
}

nav {
background-color: transparent;
}


</style>