<template>
  <div class="welcome pt-5">
    <b-col md="6" sm="12" fluid class="mx-auto mb-5">
      <h6 class="sc_item_subtitle text-center">Entenda um pouco mais</h6>
      <h2 class="title text-center">O que é a RPG Terapia?</h2>
      <iframe
        width="100%"
        height="500"
        src="https://www.youtube.com/embed/ETYlpjRwad4?si=a3h_2sesszHH0Nhe"
        title="YouTube video player"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
        referrerpolicy="strict-origin-when-cross-origin"
        allowfullscreen
      ></iframe>
    </b-col>

    <b-col md="8" sm="12" class="mx-auto">
      <b-row>
        <b-col md="6" sm="12">
          <img src="../../public/img/img-4-oquee.jpg" />
        </b-col>
        <b-col md="6" sm="12">
          <h6 class="sc_item_subtitle">Eficácia da RPG Terapia</h6>
          <h2 class="title">
            Você sabia que existem diversas evidências científicas que sugerem a
            eficácia da RPG Terapia como uma ferramenta terapêutica?
          </h2>
          <div class="text">
            <ul>
              <li>
                1. Redução de sintomas de ansiedade e depressão: Um estudo
                publicado em 2022 no International Journal of Mental Health and
                Addiction, avaliou a eficácia da RPG Terapia em pacientes com
                sintomas de ansiedade e depressão. Os resultados indicaram uma
                redução significativa dos sintomas após o tratamento com a RPG
                Terapia (Baker, Turner & Kotera, 2022).
              </li>
              <li>
                2. Melhoria da autoestima e autoeficácia: Um estudo de 2013
                publicado pela Walden University Psychology of Well-Being
                avaliou a eficácia da RPG Terapia em pacientes com baixa
                autoestima e autoeficácia. Os resultados mostraram que a RPG
                Terapia ajudou a melhorar esses indicadores e a aumentar a
                sensação de controle dos pacientes sobre suas vidas (Smith,
                2013).
              </li>
              <li>
                3. Aumento da empatia e comunicação interpessoal: Um estudo de
                2021, publicado no Journal of Research in Childhood Education
                avaliou a eficácia da RPG Terapia na melhoria da empatia e da
                comunicação interpessoal em pacientes com dificuldades nessas
                áreas. Os resultados mostraram uma melhora significativa em
                ambos os indicadores após o tratamento com a RPG Terapia (Bagès,
                Hoareau & Guerrien, 2021).
              </li>
              <li>
                4. Efeito terapêutico no transtorno do espectro autista: Um
                estudo de 2015 publicado na revista Culture, Medicine, and
                Psychiatry avaliou a eficácia da RPG Terapia em pacientes com
                transtorno do espectro autista. Os resultados indicaram que a
                RPG Terapia teve um efeito terapêutico positivo em diversas
                áreas, incluindo a melhoria das habilidades sociais e de
                comunicação (Fein, 2015).
              </li>
              <li>
                5. Melhoria da resiliência e adaptação às mudanças: Um estudo de
                2018 publicado no livro Role-Playing Game Studies avaliou a
                eficácia da RPG Terapia na melhoria da resiliência e adaptação
                às mudanças em pacientes que enfrentavam mudanças significativas
                em suas vidas. Os resultados indicaram que a RPG Terapia ajudou
                a melhorar a resiliência e a capacidade de adaptação desses
                pacientes (Bowman & Lieberoth, 2018).
              </li>
            </ul>
            <p></p>
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
.welcome ul {
  list-style: none;
  padding-left: 0;
}

.welcome ul li {
  margin-bottom: 10px;
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
