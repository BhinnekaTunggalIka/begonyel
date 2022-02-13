<template>
  <div id="ProductDetail">
    <Header/>
    <div class="container">
      <div class="row">
        <div class="col">
          <nav aria-label="breadcrumb">
            <ol class="breadcrumb">
              <li class="breadcrumb-item">
                <i class="fas fa-home"></i>&ensp;
                <a class="breadcrumb-item" href="#/landingpage">Home</a>
              </li>
              <li class="breadcrumb-item" aria-current="page">
                <b>Product Detail</b>
              </li>
            </ol>
          </nav>
        </div>
      </div>
      <Pesanan/>
      <Card2/>
      <Footer/>
    </div>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import Pesanan from "@/components/Pesanan.vue";
import Card2 from "@/components/Card2.vue";
import Footer from "@/components/Footer.vue";

export default {
  name: "ProductDetail",
  components: {
    Header,
    Pesanan,
    Card2,
    Footer
  },
};
</script>