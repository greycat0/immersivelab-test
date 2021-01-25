<template>
  <div class="absolute card bottom-10 right-10">
    <div
      class="absolute text-white right-0"
      style="font: 100px BebasNeue; top: -40px"
    >
      AK-47
    </div>
    <img class="absolute -left-20 -bottom-10" src="/immersivelab-test/img/gun.png">
    <div class="absolute card right-5 bue-button">Купить</div>
  </div>
</template>

<script>
export default {};
</script>

<style>
@font-face {
  font-family: BebasNeue;
  src: url(../assets/font/BebasNeue-Regular.woff2);
}
@font-face {
  font-family: Rubik;
  src: url(../assets/font/Rubik-VariableFontwght.woff2);
}
.card {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 10px;
  position: absolute;
  width: 300px;
  height: 130px;
}
.card::before {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: -1;
  transform: skew(-15deg);
  border: 1px solid #2b2c38;
  border-radius: 8px;
}
.bue-button {
  width: 140px;
  height: 50px;
  bottom: -35px;
  color: white;
  font-family: Rubik;
  font-weight: bold;
}
.bue-button::before {
  background: #5581ee;
}
</style>