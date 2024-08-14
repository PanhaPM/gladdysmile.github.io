<template>
    <swiper
      :slidesPerView="3"
      :spaceBetween="30"
      :freeMode="true"
      :pagination="{
        clickable: true,
      }"
      :modules="modules"
      class="mySwiper"
    >
      <swiper-slide><img src="/src/assets/img/about 1.jpg" alt=""></swiper-slide>
      <swiper-slide><img src="/src/assets/img/about 2.jpg" alt=""></swiper-slide>
      <swiper-slide><img src="/src/assets/img/about 4.jpg" alt=""></swiper-slide>
      <swiper-slide><img src="/src/assets/img/about 5.jpg" alt=""></swiper-slide>
      <swiper-slide><img src="/src/assets/img/about 6.jpg" alt=""></swiper-slide>
      <swiper-slide><img src="/src/assets/img/about 7.jpg" alt=""></swiper-slide>
      <swiper-slide><img src="/src/assets/img/air-jordan.png" alt=""></swiper-slide>
      <swiper-slide><img src="/src/assets/img/anua .jpg" alt=""></swiper-slide>
      <swiper-slide><img src="/src/assets/img/axis-y.jpg" alt=""></swiper-slide>
    </swiper>
  </template>
  <script>
    // Import Swiper Vue.js components
    import { Swiper, SwiperSlide } from 'swiper/vue';
  
    // Import Swiper styles
    import 'swiper/css';
  
    import 'swiper/css/free-mode';
    import 'swiper/css/pagination';
  
    import './style.css';
  
    // import required modules
    import { FreeMode, Pagination } from 'swiper/modules';
  
    export default {
      components: {
        Swiper,
        SwiperSlide,
      },
      setup() {
        return {
          modules: [FreeMode, Pagination],
        };
      },
    };
  </script>