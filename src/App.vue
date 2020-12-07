<template>
  <div id="root" class="">
    <div class="w-screen h-screen flex flex-col background-filters">
      <top-header :screenWidth="screenWidth" @open="open = !open" />
      <main class="flex flex-grow">
        <main-menu
          style="margin-top: 1vw"
          :open="open"
          @close="open = false"
          :screenWidth="screenWidth"
        />
        <person />
        <div style="margin-right: 5vw; margin-top: 1vw">
          <p style="color: #444553; font-family: GothamPro">ID 15782</p>
          <progress-bar />
          <carts class="mt-10" />
        </div>
      </main>
      <persons class="absolute bottom-5 left-10" />
      <offer v-if="screenWidth > 920" />
    </div>
  </div>
</template>

<script>
import Vue from "vue";
import { Drawer, Icon } from "ant-design-vue";
import "ant-design-vue/lib/drawer/style/css";

import TopHeader from "./components/TopHeader";
import MainMenu from "./components/MainMenu";
import Persons from "./components/Persons";
import Person from "./components/Person";
import ProgressBar from "./components/ProgressBar";
import Carts from "./components/Carts";
import Offer from "./components/Offer";

Vue.use(Drawer);
Vue.use(Icon);
export default {
  name: "App",
  components: {
    TopHeader,
    MainMenu,
    Persons,
    Person,
    ProgressBar,
    Carts,
    Offer,
  },
  data() {
    return {
      open: false,
      screenWidth: window.innerWidth,
    };
  },
  mounted() {
    window.onresize = () => {
      this.screenWidth = window.innerWidth;
    };
  },
};
</script>

<style>
@font-face {
  font-family: GothamPro;
  src: url(assets/font/GothamPro-Medium.woff);
}
#root {
  background: url(assets/img/background.png);
  overflow: hidden;
}
.background-filters {
  background: radial-gradient(
    63.75% 63.75% at 50% 0%,
    rgba(22, 22, 23, 0.63) 0%,
    rgba(15, 12, 20, 0.9) 70.83%
  );
  backdrop-filter: blur(15px);
}
</style>
