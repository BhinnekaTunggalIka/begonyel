<template>
  <div id="Banner">
    <div class="container">
      <div class="row">
        <div class="col-lg-6 mt-5">
          <h6 style="color: #ec982e; font-size: 20px">FoodMarket</h6>
          <br />
          <h1><b> Waktunya pilih</b></h1>
          <h1><b>menu</b> favorite <b>kamu</b></h1>
          
          <h6 style="color: #ec982e; font-size: 20px">
            mulai <b>dari</b> Rp 20.000
          </h6>
          <br />

          <router-link to="/listproduct" class="btn btn-light"
            >Lihat Menu</router-link
          >
          
          <router-link
            to="/listproduct"
            class="btn btn-warning"
            style="color: white; background-color: #ec982e"
          >
            Pesan <i class="fas fa-arrow-right"></i>
          </router-link>
        </div>
        <div class="col-lg-6 m-lg-auto">
          <img class="img" src="../assets/img_banner.png" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Banner",
};
</script>

<style>
</style>