<template>
    <div id="Success">
    <Header/>
        <div class="container">
            <div class="row mt-5 justify-content-center">
                <div class="col-lg-3 pt-5">
                    <img class="icon" src="../assets/icon.png" alt=""><br><br>
                    
                </div>
            </div>

        <div class="row justify-content-center">
                <div class="text-center col-4">
                    <h2 class="text-center" style="color:black;">Yeayy Berhasil</h2>
                    <h6 class="text-center" style=" color:#EC982E;" >Kamu akan menerima pesananmu Dalam Beberapa saat lagi</h6>
                    <br>
                    <router-link to="/listproduct" class="btn btn-primary">Pesan Kembali</router-link>
                </div>
            </div>
        </div>
    <Footer/>
    </div>
</template>

<script>
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'

export default {
    name: 'Success',
    components: {
        Header,
        Footer
    }
}
</script>