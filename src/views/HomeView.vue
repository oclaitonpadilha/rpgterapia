<template>
  <div class="home">
    <WelcomeHome msg="Welcome to Your Vue.js + TypeScript App" />
    <AboutHome msg="Welcome to Your Vue.js + TypeScript App" />
    <TestimonialsHome msg="Welcome to Your Vue.js + TypeScript App" />
    <WhoIsHome msg="Welcome to Your Vue.js + TypeScript App" />
    <JoinHome msg="Welcome to Your Vue.js + TypeScript App" />
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import WelcomeHome from "@/components/WelcomeHome.vue"; // @ is an alias to /src
import AboutHome from "@/components/AboutHome.vue"; // @ is an alias to /src
import TestimonialsHome from "@/components/TestimonialsHome.vue"; // @ is an alias to /src

import WhoIsHome from "@/components/WhoIsHome.vue"; // @ is an alias to /src
import JoinHome from "@/components/JoinHome.vue"; // @ is an alias to /src
export default Vue.extend({
  name: "HomeView",
  components: {
    WelcomeHome,
    AboutHome,
    TestimonialsHome,
    WhoIsHome,
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
