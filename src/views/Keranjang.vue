<template>
  <div id="Keranjang">
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
                <b>Keranjang</b>
              </li>
            </ol>
          </nav>
        </div>
      </div>
    </div>
  </div>
  <Table/>
  <Footer/>
  </div>
</template>

<script>

import Header from '@/components/Header.vue'
import Table from '@/components/Table.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'Keranjang',
    components: { 
        Header,
        Table,
        Footer 
        }
}
</script>

<style>

</style>