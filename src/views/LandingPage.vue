<template>
  <div class="LandingPage">
    <Header />
    <Banner />
    <Slider />
    <div class="container">
      <div class="row mt-4">
        <div class="col">
          <h4><b>Menu</b> Kami</h4>
        </div>
        <div class="col text-end">
          <a href="#/listproduct"
            ><h4><i class="far fa-eye"></i> Lihat Semua</h4></a
          >
        </div>
      </div>
    </div>
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
import axios from "axios";
import Header from "@/components/Header.vue";
import Banner from "@/components/Banner.vue";
import Slider from "@/components/Slider.vue";
import Card from "@/components/Card.vue";
import Footer from "@/components/Footer.vue";
// @ is an alias to /src

export default {
  name: "LandingPage",
  components: {
    Header,
    Banner,
    Slider,
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