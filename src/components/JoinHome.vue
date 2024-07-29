<template>
  <div>
    <div class="img-div"></div>
    <div class="join">
      <b-col md="8" fluid class="mx-auto">
        <h2 class="title text-center">FAQ</h2>
        <b-row>
          <b-col md="12" sm="12">
            <div>
              <div class="text">
                <h2>Investimento</h2>
                <p>
                  O valor é de R$495 no plano mensal para a psicoterapia em
                  grupo.
                </p>
                <h2>Horário</h2>
                <p>
                  Você nos informa quais horários são adequados para sua
                  disponibilidade e nós o colocamos em um grupo que se adapte às
                  suas necessidades.
                </p>
                <h2>Duração da sessão e da aventura</h2>
                <p>
                  Cada sessão dura 2h. A campanha jogada sempre continua ao
                  longo das sessões. Não são one-shots. Em cada sessão, a
                  aventura é retomada.
                </p>
              </div>
            </div>
          </b-col>
        </b-row>
      </b-col>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "JoinHome",
  props: {
    msg: String,
  },
  data() {
    return {
      depoimentos: [
        {
          text: "A experiência da RPG Terapia me possibilitou experienciar um olhar alternativo para a minha própria consciência. Através de categorizações de personalidades depreciadas e admiradas por mim, pude notar as convergências de tais olhares em comportamentos e opiniões consolidados há tempos em minha vida. Dessa maneira, ao ser exposto a um mundo fictício composto por elementos ideológicos que atingem meu cotidiano enquanto atuo como parte de uma narrativa, tive a oportunidade de entender diversos estigmas e peculiaridades da minha personalidade.",
        },
        {
          text: "Minha experiência com as sessões está sendo excelente! Desde o primeiro momento, me sinto à vontade para manter meu próprio ritmo ao me aprofundar em quaisquer temas, dos mais triviais aos mais sensíveis. O uso do RPG traz uma perspectiva mais clara sobre a maneira como me vejo e as atitudes que tomo ou gostaria de tomar, proporcionando muito mais conforto e facilidade para detectar e expor inseguranças, frustrações e gatilhos emocionais. Assim como a identificação, a discussão sobre os pontos recém descobertos é bastante confortável, e a busca por soluções ou aceitação se torna mais leve.",
        },
        {
          text: "A experiência da RPG Terapia me possibilitou experienciar um olhar alternativo para a minha própria consciência. Através de categorizações de personalidades depreciadas e admiradas por mim, pude notar as convergências de tais olhares em comportamentos e opiniões consolidados há tempos em minha vida. Dessa maneira, ao ser exposto a um mundo fictício composto por elementos ideológicos que atingem meu cotidiano enquanto atuo como parte de uma narrativa, tive a oportunidade de entender diversos estigmas e peculiaridades da minha personalidade.",
        },
      ],
    };
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.wpb_single_image .vc_figure {
  display: inline-block;
  vertical-align: top;
  margin: 0;
  max-width: 100%;
}
.wpb_single_image .vc_single_image-wrapper {
  display: inline-block;
  vertical-align: top;
  max-width: 100%;
}
.wpb_single_image img {
  height: auto;
  max-width: 100%;
  vertical-align: top;
}
.img-div {
  background: transparent url("../../public/img/bottom_brown-1024x52.png");
  background-repeat: repeat-x;
  min-height: 4vh;
  padding-top: 70px;
  background-size: contain;
}
.join {
  background: #e8d3b6;
  background: #f2e0c8 url("../../public/img/bw-1.jpg");
  background-repeat: repeat-x;
  color: #71675a;
  min-height: 60vh;
  padding-top: 95px;
  background-size: cover;
}

.join .title,
.join .text {
  color: #f2e0c8;
}

.join span {
  font-size: 20px;
}

@media (max-width: 600px) {
  .join {
    padding-top: 0;
  }
  .img-div {
    padding-top: 0px;
    background-size: cover;
  }

  .pt-5 {
    padding-top: 1rem;
  }
}
</style>
