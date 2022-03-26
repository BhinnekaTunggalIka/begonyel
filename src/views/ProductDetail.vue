<template>
  <div id="ProductDetail">
    <Header />
    <div class="container">
      <div class="row">
        <div class="col">
          <nav aria-label="breadcrumb">
            <ol class="breadcrumb">
              <li class="breadcrumb-item">
                <i class="fas fa-home"></i>&ensp;
                <a class="breadcrumb-item" href="#/">Home</a>
              </li>
              <li class="breadcrumb-item" aria-current="page">
                <b>Product Detail</b>
              </li>
            </ol>
          </nav>
        </div>
      </div>
      <Pesanan />
      <Card />
      <Footer />
    </div>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Pesanan from "@/components/Pesanan.vue";
import Card from "@/components/Card.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "ProductDetail",
  components: {
    Header,
    Pesanan,
    Card,
    Footer,
  },
};
</script>