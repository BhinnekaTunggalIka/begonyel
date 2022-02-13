<template>
  <div id="Header">
    <nav class="navbar navbar-expand-lg navbar-light ">
      <div class="container">
          <a class="navbar-brand" href="#"><img class="logo" src="../assets/logo_begonyel.png" alt=""></a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNavAltMarkup"
          aria-controls="navbarNavAltMarkup"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse justify-content-end" id="navbarNavAltMarkup">
          <div class="navbar-nav">
            <a class="nav-link active" aria-current="page" href="#/landingpage">Home</a>
            <a class="nav-link" href="#/listproduct">Menu Makanan</a>
            <a class="nav-link" href="#/keranjang">Keranjang <i class="fas fa-shopping-bag"></i></a>
          </div>
        </div>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style>
</style>