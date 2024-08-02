<template>
  <div class="home">
    <HeaderHome />
    <SectionTwo />
    <TestimonialsHome />
    <SessionSix />
    <JoinHome />
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import HeaderHome from "@/components/HeaderHome.vue"; // @ is an alias to /src
import SectionTwo from "@/components/SectionTwo.vue"; // @ is an alias to /src
import TestimonialsHome from "@/components/TestimonialsHome.vue"; // @ is an alias to /src

import SessionSix from "@/components/SectionSix.vue"; // @ is an alias to /src
import JoinHome from "@/components/JoinHome.vue"; // @ is an alias to /src
export default Vue.extend({
  name: "HomeView",
  components: {
    HeaderHome,
    SectionTwo,
    TestimonialsHome,
    SessionSix,
    JoinHome,
  },
  data() {
    return {
      swiperOptions: {
        loop: true,
        pagination: {
          el: ".swiper-pagination",
        },
        navigation: {
          nextEl: ".swiper-button-next",
          prevEl: ".swiper-button-prev",
        },
        autoplay: {
          delay: 5000,
        },
      },
    };
  },
});
</script>
