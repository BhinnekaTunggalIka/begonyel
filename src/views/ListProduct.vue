<template>
  <div id="ListProduct">
    <Header/>
    <div id="Breadcumb">
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
                <b>Product List</b>
              </li>
            </ol>
          </nav>
        </div>
      </div>
    </div>
  </div>
    <SearchBar/>
    <Card2/>
    <Card3/>
    <Footer/>
  </div>
</template>

<script>
import Header from "@/components/Header.vue"
import SearchBar from '@/components/SearchBar.vue'
import Card2 from '@/components/Card2.vue'
import Card3 from '@/components/Card3.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: "ListProduct",
  components: {
    Header,
    SearchBar,
    Card2,
    Card3,
    Footer
  },
};
</script>

<style>
    #ListProduct a{
        text-decoration: none;
    }
</style>