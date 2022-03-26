<template>
  <div id="CardProduct2">
    <div class="container">
      <div class="row mt-lg-5">
        <div
          class="col-lg-3 col-md-3 col-sm-3"
          v-for="item in menu"
          :key="item.id"
        >
          <div class="Card" style="width: 100%">
            <img src="../assets/lontong.png" class="card-img-top" alt="..." />
            <div class="card-body text-center">
              <h5 class="card-title">Es Buah Everest</h5>
              <p class="card-text">Harga : Rp 15.000</p>
              <router-link to="/productdetail" class="btn btn-primary"
                >Pesan Sekarang <i class="fas fa-arrow-right"></i
              ></router-link>
            </div>
          </div>
        </div>

        <!-- <div class="col">
          <div class="Card" style="width: 100%">
            <img src="../assets/lontong.png" class="card-img-top" alt="..." />
            <div class="card-body text-center">
              <h5 class="card-title">Es Buah Everest</h5>
              <p class="card-text">Harga : Rp 15.000</p>
              <router-link to="/productdetail" class="btn btn-primary"
                >Pesan Sekarang <i class="fas fa-arrow-right"></i
              ></router-link>
            </div>
          </div>
        </div>

        <div class="col">
          <div class="Card" style="width: 100%">
            <img src="../assets/lontong.png" class="card-img-top" alt="..." />
            <div class="card-body text-center">
              <h5 class="card-title">Es Buah Everest</h5>
              <p class="card-text">Harga : Rp 15.000</p>
              <router-link to="/productdetail" class="btn btn-primary"
                >Pesan Sekarang <i class="fas fa-arrow-right"></i
              ></router-link>
            </div>
          </div>
        </div>

        <div class="col">
          <div class="Card" style="width: 100%">
            <img src="../assets/lontong.png" class="card-img-top" alt="..." />
            <div class="card-body text-center">
              <h5 class="card-title">Es Buah Everest</h5>
              <p class="card-text">Harga : Rp 15.000</p>
              <router-link to="/productdetail" class="btn btn-primary"
                >Pesan Sekarang <i class="fas fa-arrow-right"></i
              ></router-link>
            </div>
          </div>
        </div> -->
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";

export default {
  name: "CardProduct2",

  data() {
    return {
      //sama seperti return view, compact()
      menu: [], //ini compact()
    };
  },
  method: {},

  mounted() {
    // this.getMenu();

    //sama seperti controller::class, yang di dalam class nya ada banyak fungsi
    axios
      .get("http://localhost:8888/begonyel/public/api/products")
      .then((response) => {
        this.menu = response.data;
        console.log(this.menu);
      })
      .catch((error) => {
        console.log(error);
      });
  },
};
</script>