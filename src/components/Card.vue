<template>
  <div id="CardProduct">
    <div class="Card" style="width: 100%">
      <img src="../assets/nasi-rames1.png" class="card-img-top" alt="..." />
      <div class="card-body text-center">
        <h5 class="card-title">{{ menu.name }}</h5>
        <p class="card-text">Harga : Rp {{ menu.price }}</p>
        <router-link to="/productdetail" class="btn btn-primary"
          >Pesan Sekarang <i class="fas fa-arrow-right"></i
        ></router-link>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardProduct",
  props: ["menu"],
};
</script>