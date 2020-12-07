<template>
  <div>
    <div class="flex">
      <div class="hexagon flex justify-center items-center text-white">
        <a-icon type="bank" />
      </div>
      <div>
        <div class="title">ОРГАНИЗАЦИЯ</div>
        <div class="body">Los Santos Police Departament (LSPD)</div>
      </div>
    </div>

    <div class="flex mt-5">
      <div class="hexagon flex justify-center items-center text-white">
        <a-icon type="audit" />
      </div>
      <div>
        <div class="title">ДОЛЖНОСТЬ В ОРГАНИЗАЦИИ</div>
        <div class="body">Начальник департамента</div>
      </div>
    </div>

    <div class="flex mt-5">
      <div class="hexagon flex justify-center items-center text-white">
        <a-icon type="dollar" />
      </div>
      <div>
        <div class="title">ДЕНЕГ НА РУКАХ</div>
        <div class="body">$5,926 842</div>
      </div>
    </div>

    <div class="flex mt-5">
      <div class="hexagon flex justify-center items-center text-white">
        <a-icon type="credit-card" />
      </div>
      <div>
        <div class="title">ДЕНЕГ В БАНКЕ</div>
        <div class="body">$2,514 367</div>
      </div>
    </div>

    <div class="flex mt-5">
      <div class="hexagon flex justify-center items-center text-white">
        <a-icon type="clock-circle" />
      </div>
      <div>
        <div class="title">ВРЕМЯ В ИГРЕ</div>
        <div class="body">18 ч. 36 мин.</div>
      </div>
    </div>
  </div>
</template>

<script>
import Vue from "vue";
import { Icon } from "ant-design-vue";
Vue.use(Icon);
export default {};
</script>

<style>
@font-face {
  font-family: Gotham;
  src: url(../assets/font/GothamPro-Medium.woff);
}
.title {
  color: #72757d;
  font: 12px Gotham;
}
.body {
  margin-top: 5px;
  color: white;
  font: 1.2rem Gotham;
}

.hexagon {
  position: relative;
  width: 30px;
  height: 17.32px;
  background-color: transparent;
  margin: 8.66px 0;
  margin-right: 10px;
  border-left: solid 2px #4f5467;
  border-right: solid 2px #4f5467;
}

.hexagon:before,
.hexagon:after {
  content: "";
  position: absolute;
  z-index: 1;
  width: 21.21px;
  height: 21.21px;
  -webkit-transform: scaleY(0.5774) rotate(-45deg);
  -ms-transform: scaleY(0.5774) rotate(-45deg);
  transform: scaleY(0.5774) rotate(-45deg);
  background-color: inherit;
  left: 2.3934px;
}

.hexagon:before {
  top: -10.6066px;
  border-top: solid 2.8284px #4f5467;
  border-right: solid 2.8284px #4f5467;
}

.hexagon:after {
  bottom: -10.6066px;
  border-bottom: solid 2.8284px #4f5467;
  border-left: solid 2.8284px #4f5467;
}
</style>