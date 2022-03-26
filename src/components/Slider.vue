<template>
  <div id="Slider">
    <div class="container mt-5">
      <div class="row">
        <div class="col-12">
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
                <img src="../assets/img_slider.png" class="d-block w-100" />
                <div class="layer m-3">
                  <h1><b>Today,</b></h1>
                  <h1><b>All</b> You</h1>
                  <h1>Can <b>Eat</b></h1>
                </div>
              </div>
              <div class="carousel-item p-3">
                <img src="../assets/img_slider.png" class="d-block w-100" />
                <div class="layer m-3">
                  <h1><b>Today,</b></h1>
                  <h1><b>All</b> You</h1>
                  <h1>Can <b>Eat</b></h1>
                </div>
              </div>
              <div class="carousel-item p-3">
                <img src="../assets/img_slider.png" class="d-block w-100" />
                <div class="layer m-3">
                  <h1><b>Today,</b></h1>
                  <h1><b>All</b> You</h1>
                  <h1>Can <b>Eat</b></h1>
                </div>
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
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Slider",
};
</script>

<style>
</style>