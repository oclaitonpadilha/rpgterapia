<template>
  <div class="welcome pt-5">
    <b-col md="8" sm="12" class="mx-auto">
      <b-row>
        <b-col md="6" sm="12">
          <img src="../../public/img/img-4-oquee.jpg" />
        </b-col>
        <b-col md="6" sm="12">
          <h6 class="sc_item_subtitle">Bem Vindo!</h6>
          <h2 class="title">
            Você sabia que pode melhorar sua saúde mental jogando RPG?
          </h2>
          <div class="text">
            <p>
              A RPGTerapia é uma abordagem inovadora que utiliza jogos de RPG
              como meio terapêutico. Neste método, os participantes assumem
              personagens e vivem aventuras fictícias que refletem desafios e
              situações da vida real. Essa prática ajuda no desenvolvimento de
              habilidades sociais, resolução de problemas, empatia e
              autoconhecimento.
            </p>
            <p>
              Esse método construído a partir de uma prática baseada em
              evidências cientificas foi fundamentado a partir de anos de
              pesquisa rigorosa, utilizando fontes confiáveis da literatura
              científica e dados clínicos de sua experiência profissional, o que
              se adequou perfeitamente com a abordagem prática e focada em
              soluções da Terapia Cognitivo-Comportamental (TCC).
            </p>
          </div>
        </b-col>
      </b-row>
    </b-col>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "WelcomeHome",
  props: {
    msg: String,
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.welcome {
  background: #f2e0c8 url("../../public/img/img92.jpg");
  background-repeat: no-repeat;
  background-position: top left;
}

.welcome img {
  height: auto;
  vertical-align: top;
  max-width: 100%;
}
.title,
.sc_item_subtitle {
  text-align: left;
}
.text {
  margin-top: 1.75em;
  text-align: left;
}
</style>
