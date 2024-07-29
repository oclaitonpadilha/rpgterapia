<template>
  <div id="app">
    <b-navbar toggleable="lg" type="dark" variant="dark" fixed="top">
      <b-navbar-brand href="#">NavBar</b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item href="#">Link</b-nav-item>
          <b-nav-item href="#" disabled>Disabled</b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
    <b-container class="main" fluid>
      <div class="header">
        <nav>
          <router-link to="/">Home</router-link> |
          <router-link to="/about">About</router-link>
        </nav>

        <div class="textHeader">
          <p>Bem Vindo a</p>
          <img src="../public/img/Logo-Branco-1024x593.png" />
          <b-container>
            <p>
              Descubra como os jogos de RPG podem transformar sua vida, e
              explorar seu potencial em um ambiente seguro e divertido.
            </p>
          </b-container>
        </div>
      </div>

      <router-view />
      <FooterHome msg="Welcome to Your Vue.js + TypeScript App" />
    </b-container>
  </div>
</template>
<script lang="ts">
import Vue from "vue";
import FooterHome from "@/components/FooterHome.vue"; // @ is an alias to /src
export default Vue.extend({
  name: "HomeView",
  components: {
    FooterHome,
  },
});
</script>
<style>
body {
  font-family: "Montserrat", sans-serif;
}
#app {
  /*font-family: Avenir, Helvetica, Arial, sans-serif;*/
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #877c6d;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}

.main {
  /*background-color: #f2e0c8;*/
  background-color: #000;
}

.header {
  background: #333 url("../public/img/slider1-1.jpg");
  background-repeat: repeat-x;
  background-position: top center;
  min-height: 1100px;
}

.textHeader {
  color: #f2e0c8;
  font-family: "Spectral SC", serif;
  font-size: 50px;
  margin-top: 200px;
}

.textHeader img {
  max-width: 100%;
  width: 20%;
}

#app .bg-dark {
  color: #b7b7b7 !important;
  background-color: #0e0d12 !important;
}

.title {
  font-size: 3em;
  font-weight: 700;
  line-height: 1.06;
  color: #070301;
  font-family: "Spectral SC", serif;
  text-align: left;
}

.sc_item_subtitle {
  color: #bd8d4c;
  font-family: "Montserrat", sans-serif;
  text-transform: uppercase;
  font-size: 14px;
  font-weight: 600;
  letter-spacing: 2px;
  font-style: normal;
  text-align: left;
}

.text {
  font-family: "Montserrat", sans-serif;
  font-size: 100%;
  outline: 0;
  -ms-word-wrap: break-word;
  word-wrap: break-word;
  color: #877c6d;
  font-size: 20px;
  font-weight: 500;
  font-style: normal;
  line-height: 30px;
  text-decoration: none;
  text-transform: none;
  text-align: left;
}

.swiper-button-next svg,
.swiper-button-prev svg {
  color: red;
}
@media (max-width: 600px) {
  .textHeader {
    font-size: 25px; /* Aumentar o tamanho da fonte para telas pequenas */
  }

  .title {
    font-size: 2em;
  }

  .sc_item_subtitle {
    font-size: 20px;
    margin-top: 10px;
  }

  .text {
    font-size: 20px;
    line-height: 30px;
    color: #333;
  }

  .whois p {
    color: #fff;
    font-size: 1.1rem;
  }

  .whois .text h2 {
    font-size: 1.2rem;
  }

  .textHeader {
    margin-top: 350px;
  }

  .textHeader img {
    width: 75%;
  }
}
</style>
