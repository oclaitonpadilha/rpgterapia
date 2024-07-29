<template>
  <div>
    <div class="img-div" style="background-color: #f2e0c8"></div>

    <div class="testimonials">
      <b-col md="6" sm="12" fluid class="mx-auto">
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
      <b-col md="8" fluid class="mx-auto mt-5">
        <h6 class="sc_item_subtitle text-center">Depoimentos</h6>
        <h2 class="title text-center">
          Veja o que diz quem já passou pela experiência
        </h2>
        <swiper-container
          slides-per-view="1"
          speed="800"
          :autoplay="autoplay"
          loop="true"
          pagination="true"
          navigation="false"
        >
          <swiper-slide
            class="mt-3"
            v-for="(item, index) in depoimentos"
            :key="index"
          >
            <b-container class="text-testimonial">
              <span class="font-italic"> "{{ item.text }}" </span>
              <p class="text-right">
                <span class="font-italic">{{ item.name }}</span>
              </p>
            </b-container>
          </swiper-slide>
        </swiper-container>
      </b-col>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "TestimonialsHome",
  props: {
    msg: String,
  },
  data() {
    return {
      autoplay: {
        delay: 10000, // tempo em milissegundos entre as mudanças de slide (5000ms = 5 segundos)
        disableOnInteraction: false, // continua o autoplay após interação do usuário
      },
      depoimentos: [
        {
          text: "A experiência da RPG Terapia me possibilitou experienciar um olhar alternativo para a minha própria consciência. Através de categorizações de personalidades depreciadas e admiradas por mim, pude notar as convergências de tais olhares em comportamentos e opiniões consolidados há tempos em minha vida. Dessa maneira, ao ser exposto a um mundo fictício composto por elementos ideológicos que atingem meu cotidiano enquanto atuo como parte de uma narrativa, tive a oportunidade de entender diversos estigmas e peculiaridades da minha personalidade.",
          name: "Fulano",
        },
        {
          text: "Minha experiência com as sessões está sendo excelente! Desde o primeiro momento, me sinto à vontade para manter meu próprio ritmo ao me aprofundar em quaisquer temas, dos mais triviais aos mais sensíveis. O uso do RPG traz uma perspectiva mais clara sobre a maneira como me vejo e as atitudes que tomo ou gostaria de tomar, proporcionando muito mais conforto e facilidade para detectar e expor inseguranças, frustrações e gatilhos emocionais. Assim como a identificação, a discussão sobre os pontos recém descobertos é bastante confortável, e a busca por soluções ou aceitação se torna mais leve.",
          name: "Ciclano",
        },
        {
          text: "Depois de poucas sessões da RPG Terapia, eu senti que o método era diferente e muito interessante. A forma como o Manoel constrói a história faz você tomar decisões difíceis e pensar em assuntos delicados, mas em um piscar de olhos, aquilo se aplica totalmente a sua vida, a suas decisões “reais”, seus medos, crenças, desejos, sonhos e dificuldades. Cada sessão em que desenvolvemos a história, aprendo mais sobre eu mesma e me pego pensando nas decisões e em nossas discussões dias depois. Sou sempre o mais franca possível nas escolhas, pois sei que cada uma diz algo sobre mim e só assim Manoel é capaz de me ajudar. Sou muito grata por tudo que ele me ajudou a enfrentar e conquistar e agora sei que posso melhorar cada vez mais.",
          name: "Outro lá",
        },
      ],
    };
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.img-div {
  background: #f2e0c8 url("../../public/img/top_dark.png");
  background-repeat: repeat-x;
  min-height: 4vh;
  padding-top: 70px;
}
.testimonials {
  background: #e8d3b6;
  background-repeat: repeat-x;
  color: #71675a;
  min-height: 50vh;
  padding-top: 95px;
}

.testimonials span {
  font-size: 20px;
}

.swiper-button-next svg,
.swiper-button-prev svg {
  color: #71675a;
}

@media (max-width: 600px) {
  .testimonials span {
    font-size: 17px; /* Aumentar o tamanho da fonte para telas pequenas */
  }
}
</style>
