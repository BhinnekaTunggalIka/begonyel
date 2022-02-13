<template>
  <div class="LandingPage">
      <Header/>
      <Banner/>
      <Slider/>
      <div class="container">
        <div class="row mt-4">
          <div class="col">
            <h4><b>Menu</b> Kami</h4>
          </div>
          <div class="col text-end">
            <a href="#/listproduct"><h4><i class="far fa-eye"></i> Lihat Semua</h4></a>
          </div>
        </div>
      </div>
      <Card/>
      <Footer/>
  </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Banner from '@/components/Banner.vue'
import Slider from '@/components/Slider.vue'
import Card from '@/components/Card.vue'
import Footer from '@/components/Footer.vue'
// @ is an alias to /src


export default {
  name: 'LandingPage',
  components: {
    Header, 
    Banner,
    Slider,
    Card,
    Footer
  }
}
</script>