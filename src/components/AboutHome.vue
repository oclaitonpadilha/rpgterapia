<template>
  <div class="about">
    <b-col md="8" sm="12" class="mx-auto pt-5">
      <b-row>
        <b-col md="6" sm="12">
          <h6 class="sc_item_subtitle">Psicoterapia + Jogo de RPG</h6>
          <h2 class="title">O poder da RPG Terapia</h2>
          <div class="text">
            A RPGTerapia oferece uma série de benefícios, incluindo:

            <ul>
              <li>
                Ressignificação da sua história, mesmo que você nunca tenha
                feito terapia
              </li>
              <li>
                Construção de novas possibilidades de vida, ainda que você nunca
                tenha jogado RPG.
              </li>
              <li>
                Manejo da ansiedade e humor, aumentando seu equilíbrio emocional
              </li>
              <li>
                Aprimoramento de habilidades sociais, fazendo você se sentir
                capaz de evoluir
              </li>
              <li>Regulação emocional e autoestima</li>
            </ul>
          </div>
        </b-col>
        <b-col md="6" sm="12">
          <img src="../../public/img/img-15-comofunciona.jpg" />
        </b-col>
      </b-row>
    </b-col>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "AboutHome",
  props: {
    msg: String,
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.about {
  background: #f2e0c8 url("../../public/img/img-9.png");
  background-repeat: no-repeat;
  background-position: center;
  min-height: 50vh;
}
.about img {
  height: auto;
  vertical-align: top;
  max-width: 100%;
}
</style>
