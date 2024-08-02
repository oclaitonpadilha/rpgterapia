<template>
  <div>
    <b-button variant="success" size="lg" target="_BLANK" :href="url"
      >Agendar Agora</b-button
    >
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "ButtonCAT",
  props: {
    msg: String,
  },
  data() {
    const nro = "5551997820241";
    const msg = "agendar";
    return {
      url: `https://wa.me/${nro}?text=${msg}`,
    };
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.btn-lg {
  font-size: 2rem;
  padding: 1rem 1rem;
}
</style>
