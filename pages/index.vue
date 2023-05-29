<template>
  <div>
     <div>
        <nav class="container lg:px-32 px-4 py-4 mx-auto md:flex md:justify-between md:items-center fixed-top">       
          <div class="flex items-center justify-between w-full">
            <nuxtlink to="/" class="text-xl font-bold text-gray-800 md:text-2xl"> 
              <img src="/logo.png" alt="" class="h-7 hover:scale-110 duration-100">
            </nuxtlink>
            <!-- Mobile menu button -->
            <div @click="showMenu = !showMenu" class="flex md:hidden">
              <button type="button" class="text-gray-800 hover:text-gray-400 focus:outline-none focus:text-gray-400">           
                <svg viewBox="0 0 24 24" class="w-6 h-6 fill-current">
                  <path fill-rule="evenodd" d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z"/>
                </svg>
              </button>
            </div>
          </div>
          <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
          <ul :class="showMenu ? 'flex' : 'hidden'" class=" flex-col mt-8 space-y-4 md:flex md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0">
            <li class=" font-bold text-purple-700 hover:scale-110 duration-100">
              <a href="#home">Beranda</a> 
            </li>
            <li class=" font-bold text-gray-500 hover:scale-110 mx-2 duration-100">
              <a href="#tentang kami">Tentang</a> 
            </li>
            <li class=" font-bold text-gray-500 hover:scale-110 mx-2 duration-100">
              <a href="#layanan">Layanan</a> 
            </li>
            <li class=" font-bold text-gray-500 hover:scale-110 mx-2 duration-100">
              <a href="#blog"> Blog</a>
            </li>
            <li class=" font-bold text-gray-500 hover:scale-110 mx-2 duration-100">
              <a href="">Kontak</a>
            </li>
            <button class="text-white hover:outline py-3 px-3 hover:scale-110 duration-100 bg-purple-600 rounded-full hover:shadow-lg hover:opacity-80 transition ease-in-out">
              CobaGratis         
            </button>
          </ul>
        </nav>
        <div @click="toggleNav" class="flex md:hidden">
          <button type="button" class="text-gray-800 hover:text-gray-900 focus:outline-none focus:text-gray-900" aria-label="toggle menu" />                        
        </div>
     </div>    
    <section id="home" class="px-3 lg:px-40 lg:py-20 bg-purple-100">
      <div class="container w-full">
        <div class="flex flex-wrap">
          <div class="w-full self-center lg:w-1/2 md:w-1/2">
            <h1 class=" font-bold text-black" style="font-size: 3.3rem;">
                Nikmati Pelayanan Cepat & Tanpa Ribet
            </h1>
            <p class="font-base pt-10 text-slate-600 mb-8 leading-relaxed md:text-sm">Aplikasi Chabot “IzinPak” siap melayani kebutuhan 
              <span class=" font-serif font-bold text-black">Masyarakat</span> dalam proses administrasi pemerintahan RT, RW dan Kelurahan.
            </p>
            <a href="" class="text-base text-white bg-violet-600  hover:bg-purple-700 py-3 px-3 rounded-lg hover:shadow-lg hover:opacity-80 transition duration-300 ease-in-out">
              Coba Sekarang
            </a>
          </div>
          <div class="hidden md:block w-full  px-4 lg:w-1/2 sm:w-8 md:w-1/2 ">
            <div class="relative mt-5 lg:mt-1 lg:right-0">
              <img src="/ijin.png" alt="" class="mx-auto object-contain h-150 w-96"/>
            </div>
          </div>
        </div>
      </div>
    </section>    
    <section  id="tentang kami" class=" bg-purple-100"  >
      <div class="container px-3 lg:px-40 py-10" >
        <div class="flex flex-wrap">
          <div class="w-full self-center" data-aos="fade-right" data-aos-duration="2500">
            <p class="font-semibold text-base text-gray-600 ">
              Tentang kami
            </p>
            <h2 class="font-bold text-purple-700 text-3xl ">
              Mengenal Izinpak
            </h2>
            <p class=" mt-4 font-semibold text-slate-500">
              Aplikasi Chabot “IzinPak” siap melayani kebutuhan Masyarakat dalam proses administrasi pemerintahan RT, RW dan Kelurahan.Aplikasi Chabot “IzinPak” siap melayani kebutuhan Masyarakat dalam proses administrasi pemerintahan
            </p>
          </div>
        </div>
      </div>
      <div  class="relative" data-aos="fade-up" data-aos-duration="3000">
        <div class="absolute bottom-0 left-0 h-1/2 w-full bg-white"/>
          <div class="relative py-12 rounded-r-full bg-purple-300">
            <div class="grid grid-cols-12 gap-4 md:gap-8">
              <div class="col-span-6 lg:col-span-3 text-center"  >         
                <div class="flex justify-center items-center w-16 h-16 rounded-2xl mx-auto bg-white text-purple-600 font-bold italic" style="font-size: 2rem;">01</div>        
                <div class="font-semibold mt-4" style="font-size: 1.3rem;"> Digitalisasi</div>       
                <p class="mt-2 text-gray-500">
                  Memindahkan proses Administrasi dan Pelayanan Publik ke layanan digital.
                </p>   
              </div>             
              <div class="col-span-6 lg:col-span-3 text-center">
                <div class="flex justify-center items-center w-16 h-16 rounded-2xl mx-auto bg-white text-purple-600 font-bold italic" style="font-size: 2rem;">02</div> 
                <div class="font-semibold mt-4" style="font-size: 1.3rem;">Melayani</div>
                <p class="mt-2 text-gray-500">
                  Mempermudah kinerja Pemerintah dalam melayani segala kebutuhan masyarakat.
                </p>
              </div>
              <div class="col-span-6 lg:col-span-3 text-center">
                <div class="flex justify-center items-center w-16 h-16 rounded-2xl mx-auto bg-white text-purple-600 font-bold italic" style="font-size: 2rem;">03</div>       
                <div class="font-semibold mt-4" style="font-size: 1.3rem;">Terbuka</div> 
                <p class="mt-2 text-gray-500">
                  Menyediakan akses komunikasi terbuka untuk mempermudah  menyampaikan informasi.
                </p>
              </div>
              <div class="col-span-6 lg:col-span-3 text-center">
                <div class="flex justify-center items-center w-16 h-16 rounded-2xl mx-auto bg-white text-purple-600 font-bold italic" style="font-size: 2rem;">04</div>
                <div class="font-semibold mt-4" style="font-size: 1.3rem;">Transparansi</div>
                <p class="mt-2 text-gray-500">
                  Terwujudnya komunikasi dua arah  yang lebih transparan antara Pemerintah dengan masyarakat.
                </p> 
              </div>
            </div>
          </div>
      </div>      
    </section>
    <section id="layanan" class="px-3  py-10 bg-white">
      <div class="container">
        <div class="lg:flex lg:flex-row">
          <div class="w-full self-center" 
          data-aos="flip-left" data-aos-duration="1500">
             <img src="/hp.png" alt="" class="pt-20 hidden md:block md:px-60">
          </div>
            <div class="relative" data-aos="flip-right" data-aos-duration="1500">
              <img src="/logo.png" alt="">
              <h2 class="mt-5 font-bold" style="font-size: 2rem;">
                Produk & Layanan
              </h2>
              <p class="mt-5 text-slate-600">
                Aplikasi Chabot “IzinPak” siap melayani kebutuhan Masyarakat dalam proses administrasi pemerintahan RT, RW dan Kelurahan.
              </p>            
              <div class="flex items-start w-full p-4">
                <h1 class="font-bold italic text-purple-700"  style="font-size: 2rem;">
                  01
                </h1>
                <div class="ml-8">
                  <div class="font-semibold items-center" style="font-size: 1.5rem;">Layanan Surat</div>  
                  <div class="text-slate-600">Memindahkan proses Administrasi dan Pelayanan Publik ke layanan digital.</div>
                </div>     
              </div> 
              <div class="flex items-start w-full p-4">
                <h1 class="font-bold italic text-purple-700"  style="font-size: 2rem;">
                  02
                </h1>
                <div class="ml-8">
                  <div class="font-semibold items-center" style="font-size: 1.5rem;">Tanya Jawab</div>  
                  <div class="text-slate-600">Memindahkan proses Administrasi dan Pelayanan Publik ke layanan digital.</div>
                </div>     
              </div> 
              <div class="flex items-start w-full p-4">
                <h1 class="font-bold italic text-purple-700"  style="font-size: 2rem;">
                  03
                </h1>
                <div class="ml-8">
                  <div class="font-semibold items-center" style="font-size: 1.5rem;">Pelaporan</div>  
                  <div class="text-slate-600">Memindahkan proses Administrasi dan Pelayanan Publik ke layanan digital.</div>
                </div>     
              </div> 
            </div>
        </div>
      </div>
    </section>
    <section id="blog" class="pt-36 pb-32 bg-purple-100">
        <div class="w-full">
          <div class="mx-w-xl mx-auto text-center mb-16">
            <h2 class="font-bold text-black  text-3xl">
              <span class="text-purple-500 font-bold">Blog</span> Dari Kami Yang Membuat Anda <span class="text-purple-500">Akan Terus Updated</span>
            </h2>
          </div>
        </div>
          <div class="flex lg:px-32 flex-wrap">
            <div class="w-full px-4 md:w-1/2 xl:w-1/3 mb-7 ">
              <div class="bg-white rounded-xl shadow-lg overflow-hidden">
                <img src="https://www.qhomemart.com/blog/wp-content/uploads/2021/01/media-hidroponik-768x500.png" alt="" class="w-full">
                <div class="py-8 px-6">
                  <h3>
                   <a href="" class="rounded-full py-2 px-3 bg-yellow-300 text-center font-bold text-black">News</a>
                  </h3>
                  <p class="font-semibold pt-3 mb-6">
                    Indor Farming Wujud Pertanian Masa Depan Untuk Indonesia.
                  </p>
                  <p class="text-slate-600 font-semibold pt-2 mb-6">
                    Indor Farming Wujud Pertanian Masa Depan Untuk Indonesia.
                  </p>
                  <a href="" class=" text-purple-500 pt-4">Baca Selengapnya</a>
                </div>
              </div>
            </div>
            <div class="w-full px-4 md:w-1/2 xl:w-1/3 mb-7 ">
              <div class="bg-white rounded-xl shadow-lg overflow-hidden">
                <img src="https://tse3.mm.bing.net/th?id=OIP.swLRokI6cY-hIreqOEO63AHaE8&pid=Api&P=0" alt="" class="w-full">
                <div class="py-8 px-6">
                  <h3>
                   <a href="" class="rounded-full py-2 px-3 bg-yellow-300 text-center font-bold text-black">tips</a>
                  </h3>
                  <p class="font-semibold pt-3 mb-6">
                    Pepaya California sangat mudah untuk dibudidayakan.
                  </p>
                  <p class="text-slate-600 font-semibold pt-2 mb-6">
                    Pepaya California sangat mudah untuk dibudidayakan.
                  </p>
                  <a href="" class=" text-purple-500 pt-4">Baca Selengapnya</a>
                </div>
              </div>
            </div>
            <div class="w-full px-4 md:w-1/2 xl:w-1/3 ">
              <div class="bg-white rounded-xl shadow-lg overflow-hidden">
                <img src="https://assets-a2.kompasiana.com/items/album/2020/10/30/money-kompas-com-5e99204d9dc6a-5f9c14bbd541df6a9d7ed6c2.jpg?t=o&v=770" alt="" class="w-full">
                <div class="py-8 px-6">
                  <h3>
                   <a href="" class="rounded-full py-2 px-3 bg-yellow-300 text-center font-bold text-black">News</a>
                  </h3>
                  <p class="font-semibold pt-3 mb-6">
                    Mengapa sawah semakin “hilang” Apa penyebabnya?
                  </p>
                  <p class="text-slate-600 font-semibold pt-2 mb-6">
                    Mengapa sawah semakin “hilang” Apa penyebabnya?
                  </p>
                  <a href="" class=" text-purple-500 pt-4">Baca Selengapnya</a>
                </div>
              </div>
            </div>
            <div class="w-full px-4 md:w-1/2 xl:w-1/3 ">
              <div class="bg-white rounded-xl shadow-lg overflow-hidden">
                <img src="http://4.bp.blogspot.com/-C_VYckF9Opg/TiLhJnddYDI/AAAAAAAACOM/GuSIsppygKI/s1600/2009+Rinjani+smoke+and+crater.JPG" alt="" class="w-full">
                <div class="py-8 px-6">
                  <h3>
                   <a href="" class="rounded-full py-2 px-3 bg-yellow-300 text-center font-bold text-black">News</a>
                  </h3>
                  <p class="font-semibold pt-3 mb-6">
                    Gunung Rinjani Gunung tertinggi dengan ketinggian 3.762 mdpl.
                  </p>
                  <p class="text-slate-600 font-semibold pt-2 mb-6">
                    Gunung Rinjani Gunung tertinggi dengan ketinggian 3.762 mdpl.
                  </p>
                  <a href="" class=" text-purple-500 pt-4">Baca Selengapnya</a>
                </div>
              </div>
            </div>
          </div>
    </section>
    <section id="kolaborasi" class="bg-purple-200 py-10">
      <div class="container">
        <div class="lg:flex px-2 lg:flex-row">
          <div class="w-full self-center" data-aos="fade-right" data-aos-duration="2000">
            <img src="/buku.png" alt="" class="hidden lg:block pl-60">
          </div>
          <div class="relative pr-20" data-aos="fade-right" data-aos-duration="2000">
            <h2 class="mt-5 font-bold" style="font-size: 2rem;">
              Mari bergabung dan berkolaborasi!
            </h2>
            <p class="mt-5 text-slate-600">
              Silahkan isi beberapa data untuk terhubung bersama kami untuk kita berkolaborasi dan berkembang bersama memajukan pertanian Indonesia.
            </p> 
            <button class="btn rounded-lg bg bg-purple-600 text-white mt-8 px-3 py-3">Mari Bergabung</button>
          </div>            
        </div>
      </div>
    </section>
    <section id="footer" class="bg-white py-20 text-gray-400">
      <div class="container mx-auto px-4">
        <div class="footer-box flex justify-around md:flex-row flex-col lg:gap-0 gap-10 pb-10">
          <div class="box lg:w-[500px]">
            <div class="logo">
              <img src="/logo.png" alt=""> 
              <div class="mt-4">Logistik Pertanian hadir untuk merubah sistem rantai pasok pertanian jauh lebih efisien, adil, transparan and berkelanjutan</div>                   
            </div>
          </div>
          <div class="box flex flex-col lg:w-[100px] gap-2">
              <h4 class="font-bold text-black mb-3">
                Siapa Kami?
              </h4>
              <a href="#tentang kami" class=" hover:opacity-100 hover:text-purple-500">Tentang Kami</a>
              <a href="#layanan" class=" hover:opacity-100 hover:text-purple-500">Layanan</a>
              <a href="#" class=" hover:opacity-100 hover:text-purple-500">Aplikasi</a>
          </div>
          <div class="box flex flex-col lg:w[200px] gap-2">
              <h4 class="font-bold text-black ">
                kontak
              </h4>
              <p class=" hover:opacity-100 hover:text-purple-500 cursor-pointer">
                Bantuan
              </p>
              <p class=" hover:opacity-100 hover:text-purple-500 cursor-pointer">
                FAQ
              </p>
              <p class=" hover:opacity-100 hover:text-purple-500 cursor-pointer">
                Afiliasi
              </p>
          </div>
          <div class="box flex flex-col lg:w[200px] gap-2">
              <h4 class="font-bold text-black mb-3">
                Lainnya
              </h4>
              <p class=" hover:opacity-100 hover:text-purple-500 cursor-pointer">
                Blog&Info
              </p>
              <p class=" hover:opacity-100 hover:text-purple-500 cursor-pointer">
                Dukung Kami
              </p>
          </div>
        </div>
        <div class=" text-black">
          <div class="flex items-center justify-center">
            <p>
              All rights reserved@logistikpertanian.co.id
            </p>
          </div>
        </div>
      </div>
    </section>
  </div>
  </template>
<script>
  export default {
    data() {
        return {
          showMenu: false,
        };
      },
      methods: {
        toggleNav: function () {
          this.showMenu = !this.showMenu;
        },
      },
  }
</script>
