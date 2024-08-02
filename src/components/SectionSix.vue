<template>
  <div class="whois">
    <div class="img-div"></div>
    <b-col md="8" sm="12" class="mx-auto mt-5">
      <b-row>
        <b-col md="6" sm="12" class="offset-md-7 mt-5">
          <div class="pt-5">
            <h6 class="sc_item_subtitle">Como funciona a</h6>
            <h2 class="title">RPG Terapia?</h2>
            <div class="text">
              <h2>Investimento</h2>
              <p>
                De:
                <span style="text-decoration: line-through">R$ 600</span> por
                mês<br />
                Por apenas:
                <span style="font-size: 40px; color: #f2e0c8">R$ 49,90</span>
              </p>
              <p style="font-style: italic">
                Esse valor é da sessão experimental. Caso você goste da
                experiência e queira seguir no processo o valor é de apenas R$
                395 no plano mensal
              </p>
              <h2>Horário</h2>
              <p>
                Você nos informa quais horários são adequados para sua
                disponibilidade e nós o colocamos em um grupo que se adapte às
                suas necessidades.
              </p>
              <h2>Duração da sessão e da aventura</h2>
              <p>
                Cada sessão dura 2h. A campanha jogada sempre continua ao longo
                das sessões. Não são one-shots. Em cada sessão, a aventura é
                retomada.
              </p>
            </div>
          </div>
          <div class="mt-5">
            <ButtonCAT />
          </div>
        </b-col>
      </b-row>
    </b-col>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import ButtonCAT from "@/components/ButtonCAT.vue";

export default Vue.extend({
  name: "WhoIsHome",
  components: {
    ButtonCAT,
  },
  props: {
    msg: String,
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.whois {
  background: #070301 url("../../public/img/bg-cta6-copyright.jpg");
  background-repeat: no-repeat;
  background-position: center left;
  background-size: cover;
  min-height: 135vh;
}

.whois .img-div {
  background: url("../../public/img/bottom_dark.png");
  background-repeat: repeat-x;
  background-position: top left;
  background-size: cover;
  min-height: 5vh;
  padding-top: 95px;
  color: #b7b7b7;
}
.whois img {
  height: auto;
  vertical-align: top;
  max-width: 100%;
}

.sc_item_subtitule,
.title,
h2 {
  color: #f2e0c8;
}
</style>
