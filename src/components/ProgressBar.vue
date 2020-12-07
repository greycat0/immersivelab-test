<template>
  <div>
    <div class="flex text-white my-3" style="font-family: GothamPro">
      <div>Уровень 24</div>
      <div class="ml-auto">156 872 / 300 000</div>
    </div>
    <div class="flex">
      <div class="progress-part progress-part-active"></div>
      <div class="progress-part progress-part-active"></div>
      <div
        class="progress-part"
        style="background: linear-gradient(90deg, #3c6deb 52%, #2a2e35 53%)"
      ></div>
      <div class="progress-part"></div>
      <div class="progress-part"></div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
@font-face {
    font-family: GothamPro;
    src: url(../assets/font/GothamPro-Medium.woff);
}
.progress-part {
  margin-right: 6px;
  width: 60px;
  height: 6px;
  background: #2a2e35;
  border-radius: 1px;
  transform: skew(-10deg);
}
.progress-part-active {
  box-shadow: 0px 0px 12px rgba(93, 134, 238, 0.5);
  background: linear-gradient(180deg, #3c6deb 0%, #5d86ee 100%);
}
</style>