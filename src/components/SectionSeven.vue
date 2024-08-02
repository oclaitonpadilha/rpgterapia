<template>
  <div class="footer footer_wrap">
    <div class="mt-5">
      <ButtonCAT />
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import ButtonCAT from "@/components/ButtonCAT.vue";
export default Vue.extend({
  name: "FooterHome",
  props: {
    msg: String,
  },
  components: {
    ButtonCAT,
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.footer {
  background: #070301 url("../../public/img/bottom.png");
  background-repeat: repeat-x;
  background-size: contain;
  color: #71675a;
  min-height: 25vh;
  padding-top: 95px;
  text-align: center;
}

.widget {
  border-color: rgb(70, 70, 70);
}

.contacts_logo {
  background-color: rgb(7, 3, 1);
  color: rgb(113, 103, 90);
}
.vc_col-sm-2 {
  width: 16.6667%;
  float: left;
}

.vc_col-sm-3 {
  width: 25%;
}

.vc_column-inner {
  padding-left: 15px;
  padding-right: 15px;
  margin-top: 25px;
}

.widgettitle {
  color: rgb(242, 224, 200);
}

.footer_wrap .widgettitle {
  font-size: 1.6em;
  font-family: "Spectral SC", serif;
  font-weight: 700;
  letter-spacing: -1px;
}
.widget ul {
  padding-left: 0;
  list-style-type: none;
  margin: 0px;
}

.social_item {
  display: block;
  line-height: inherit;
  vertical-align: top;
  margin: 0px;
}
</style>
