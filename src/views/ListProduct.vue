<template>
  <div id="ListProduct">
    <Header />
    <div id="Breadcumb">
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
                  <b>Product List</b>
                </li>
              </ol>
            </nav>
          </div>
        </div>
      </div>
    </div>
    <SearchBar />
    <!-- ini adalah perintah memasukkan data ke dalam component Card -->
    <div class="container">
      <div class="row">
        <div
          class="col-lg-3 col-md-3 col-sm-3"
          v-for="item in menu"
          :key="item.id"
        >
          <Card v-bind:menu="item" />
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script>
import Header from "@/components/Header.vue";
import SearchBar from "@/components/SearchBar.vue";
import Card from "@/components/Card.vue";
import Footer from "@/components/Footer.vue";
import axios from "axios";

export default {
  name: "ListProduct",
  components: {
    Header,
    SearchBar,
    Card,
    Footer,
  },

  data() {
    return {
      menu: [],
    };
  },
  method: {},

  mounted() {
    //sama seperti controller::class, yang di dalam class nya ada banyak fungsi
    axios
      .get("http://localhost:8888/begonyel/public/api/products")
      .then((response) => {
        this.menu = response.data;
        console.log(this.menu[0].id);
      })
      .catch((error) => {
        console.log(error);
      });
  },
};
</script>

<style>
#ListProduct a {
  text-decoration: none;
}
</style>