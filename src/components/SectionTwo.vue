<template>
  <div class="about">
    <b-col md="8" sm="12" class="mx-auto pt-5">
      <b-row>
        <b-col md="6" sm="12">
          <h6 class="sc_item_subtitle">Psicoterapia + Jogo de RPG</h6>
          <h2 class="title">Como foi desenvolvido?</h2>
          <div class="text">
            <p>
              A RPG Terapia nasceu de inquietações observadas pelo Dr. Manoel
              Acioli na sua prática clínica.
            </p>

            <p>
              Ele notou que as limitações impostas pela rigidez dogmática na
              psicologia dificultavam inovações, o que motivou o desenvolvimento
              desse método.
            </p>
            <p>
              Ao longo de sua carreira, o Dr. Manoel Acioli sempre buscou romper
              com paradigmas estabelecidos, incorporando elementos lúdicos em
              sua abordagem.
            </p>
            <p>
              A gamificação do processo terapêutico foi gradualmente se tornando
              uma realidade em sua prática clínica, facilitando avanços em
              questões delicadas e aumentando a eficácia dos tratamentos.
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
