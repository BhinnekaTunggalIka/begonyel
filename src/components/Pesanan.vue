<template>
  <div id="Pesanan">
    <div class="container">
      <div class="row">
        <div class="col-4">
          <div
            id="carouselExampleIndicators"
            class="carousel slide"
            data-bs-ride="carousel"
          >
            <div class="carousel-indicators">
              <button
                type="button"
                data-bs-target="#carouselExampleIndicators"
                data-bs-slide-to="0"
                class="active"
                aria-current="true"
                aria-label="Slide 1"
              ></button>
              <button
                type="button"
                data-bs-target="#carouselExampleIndicators"
                data-bs-slide-to="1"
                aria-label="Slide 2"
              ></button>
              <button
                type="button"
                data-bs-target="#carouselExampleIndicators"
                data-bs-slide-to="2"
                aria-label="Slide 3"
              ></button>
            </div>

            <div class="carousel-inner">
              <div class="carousel-item p-3 active">
                <img
                  style="
                    border-bottom-left-radius: 20px;
                    border-bottom-right-radius: 20px;
                  "
                  src="../assets/nasi-ayam-geprek.png"
                  class="d-block w-100"
                />
              </div>

              <div class="carousel-item p-3">
                <img
                  style="
                    border-bottom-left-radius: 20px;
                    border-bottom-right-radius: 20px;
                  "
                  src="../assets/nasi-ayam-geprek.png"
                  class="d-block w-100"
                />
              </div>

              <div class="carousel-item p-3">
                <img
                  style="
                    border-bottom-left-radius: 20px;
                    border-bottom-right-radius: 20px;
                  "
                  src="../assets/nasi-ayam-geprek.png"
                  class="d-block w-100"
                />
              </div>
            </div>

            <button
              class="carousel-control-prev"
              type="button"
              data-bs-target="#carouselExampleIndicators"
              data-bs-slide="prev"
            >
              <i class="fas fa-arrow-circle-left"></i>
            </button>
            <button
              class="carousel-control-next"
              type="button"
              data-bs-target="#carouselExampleIndicators"
              data-bs-slide="next"
            >
              <i class="fas fa-arrow-circle-right"></i>
            </button>
          </div>
        </div>

        <div class="col-8 mt-lg-4">
          <h3>Nasi Geprek Klenger</h3>

          <p style="font-size: 17px; margin-top: 20px">
            Harga : <b>RP. 20.000</b>
          </p>
          <hr />
        
        <div class="jumlah">
          <p style="font-size:12px;">Jumlah Pesan</p>
          <div class="form-group">
              <label for="jumlah_pemesanan">Jumlah Pesan</label>
                <input style="width:70px;" type="number" placeholder="1" class="form-control"
              />
            </div>
        </div>

        <div class="deskripsi">
          <p style="font-size:12px;">Keterangan</p>
          <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
        </div>
        <br>
        <router-link to="/keranjang" class="btn btn-warning" > Masukan Keranjang &ensp; &ensp; &ensp;<i class="fas fa-arrow-right"></i>
        </router-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Pesanan",
};
</script>