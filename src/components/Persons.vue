<template>
  <div class="flex items-end" style="font-family: Rubik">
    <div
      class="flex items-end mx-3 person-cart h-36"
      style="background: #373f56; height: max(12vw, 10rem)"
    >
      <img src="/img/mickahel.png" />
      <span class="absolute -left-3 -bottom-2 text-white"
        >Michael <span class="font-bold">De Santa</span></span
      >
    </div>
    <div
      class="flex items-end mx-3 person-cart"
      style="
        background: #242834;
        border: 3px solid;
        border-image: linear-gradient(#5d86ee 0%, rgba(93, 134, 238, 0) 75%) 27;
        box-shadow: 0px -32px 48px rgba(93, 134, 238, 0.35);
      "
    >
      <img src="/img/isabella2.png" />
      <span
        class="absolute -left-3 -bottom-2 text-white"
        >Isabella <span class="font-bold">Brown</span></span
      >
    </div>
    <div
      class="mx-3 person-cart flex justify-center items-center empty-cart"
      style="border: 3px dashed #2b2c38; color: #2b2c38; font: 50px bold;"
    >
      +
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
@font-face {
  font-family: Rubik;
  src: url(../assets/font/Rubik-VariableFontwght.woff2);
}
.person-cart::before {
  content: "";
  position: absolute;
  top: 60%;
  left: 0;
  bottom: 0;
  right: 0;
  background: linear-gradient(transparent, rgba(0, 0, 0, 0.95));
}
.empty-cart::before {
  background: transparent;
}
.person-cart {
  border-radius: 8px;
  width: max(10vw, 8rem);
  height: max(13vw, 8rem);
  transform: skew(-4deg);
}
</style>