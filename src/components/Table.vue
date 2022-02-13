<template>
  <div id="Table">
    <div class="container">
      <div class="row">
        <div class="col-12">
          <table  class="table" style="color:#F57C00">
            <thead >
              <tr class="text-atas">
                <th style="width: 200px;">Produk</th>
                <th style="width: 150px;" >Nama</th>
                <th class="text-center" style="width: 450px;" >Keterangan</th>
                <th class="text-center" >Jumlah</th>
                <th class="text-center">Harga</th>
                <th class="text-center">Aksi</th>
              </tr>
            </thead>
            <tbody>
              <tr >
                <td ><img class="img" src="../assets/nasi-ayam-geprek.png" alt=""></td>
                <td><b>Nasi Geprek Klenger</b></td>
                <td class="text-center">pedes level 3 yaa, mantap loor</td>
                <td class="text-center">1</td>
                <td class="text-center">Rp. 20.000</td>
                <td class="text-center"><i class="fas fa-trash"></i></td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>

      <div class="row justify-content-end" style="margin-right:-110px;">
        <div class="col-3">
          <b style="color:black;">Total Harga:</b>
        </div>
        <div class="col-2 ">
          <b style="color:black;">Rp. 20.000</b>
        </div>
      </div>

      <div class="row mt-5 justify-content-end">
        <div class="col-6">
          <p style="font-size:12px;">Nama Pemesan</p>
          <input type="text" class="form-control" placeholder="Nama Pemesan" id="jumlahpesanan" >
        </div>
      </div>

      <div class="row mt-3 justify-content-end">
        <div class="col-6">
          <p style="font-size:12px;">No Meja</p>
          <input type="text" class="form-control" placeholder="1" id="jumlahpesanan" >
        </div>
      </div>

      <div class="row mt-3 justify-content-end">
        <div class="col-2">
          <router-link to="/success" class="btn btn-primary">Pesan Sekarang &ensp;<i class="fas fa-arrow-right"></i></router-link>
        </div>
      </div>

    </div>
  </div>
</template>