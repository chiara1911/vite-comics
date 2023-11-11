<template>
  <header>
    <div class="container mt-1">
      <div class="d-flex justify-content-between">
        <img src="../assets/images/dc-logo.png" alt="dc-logo" />
        <nav class="navbar navbar-expand-lg navbar-light ">
          <button
            class="navbar-toggler"
            type="button"
            data-toggle="collapse"
            data-target="#navbarNav"
            aria-controls="navbarNav"
            aria-expanded="false"
            aria-label="Toggle navigation"
          >
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarNav">
            <ul class="navbar-nav text-uppercase " v-for="navLink in navLinks">
              <li class="nav-item ">
                <a class="nav-link" href="#"
                  >{{ navLink }}</a
                >
              </li>
             
            </ul>
          </div>
        </nav>

        <!-- <ul class="d-flex flex-row justify-content-between align-items-center"> -->
          <!-- <li  class="p-1 ">
            <a href="#"></a>
          </li> -->
        
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: "HeaderApp",

  data() {
    return {
      navLinks: [
        "characters",
        "comics",
        "movies",
        "tv",
        "games",
        "collectibles",
        "videos",
        "fans",
        "news",
        "shop",
      ],
    };
  },
};
</script>

<style lang="scss"></style>
