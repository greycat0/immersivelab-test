<template>
  <div class="flex text-white m-1 mr-14" style="font-family: GothamPro">
    <div class="item" style="width: 108px">
      <a-icon class="text-2xl" type="team" />
      <span class="text-base -mb-1">18</span>
      <span
        class="rounded-full w-2 h-2 ml-2"
        style="background-color: #84db82"
      ></span>
    </div>
    <div class="item relative">
      <span
        class="absolute top-0 -right-2 rounded-full w-5 h-4 text-xs text-center"
        style="background-color: #ff4848"
        >7</span
      >
      <a-icon class="text-2xl" type="bell" />
    </div>
    <div class="item">
      <a-icon class="text-2xl" type="setting" />
    </div>
    <div class="item">
      <div class="avatar-item">
        <img
          style="transform: skew(15deg)"
          src="/img/avatar.png"
          alt="avatar"
        />
      </div>
    </div>
    <div class="relative" style="margin: 10px">
      <div>ex3dervolga</div>
      <div class="flex items-center ml-6" style="color: #ffd600">
        <span
          class="absolute bottom-2 -left-3 rounded-full w-4 h-4 ml-2 z-10"
          style="background-color: #ffd600; border: 2px solid #14121a"
        ></span>
        <span
          class="absolute bottom-4 -left-1 rounded-full w-3 h-3 ml-2"
          style="background-color: #ffd600"
        ></span>
        <div>5607</div>
        <div class="item gold-button"><span class="-mb-1">+</span></div>
      </div>
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
.item {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 10px;
  position: relative;
  width: 57px;
  height: 48px;
}
.item::before {
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

.avatar-item {
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: -1;
  transform: skew(-15deg);
  border: 1px solid #2b2c38;
  border-radius: 8px;
  overflow: hidden;
}
.gold-button {
  width: 36px;
  height: 24px;
  margin: 0;
  margin-left: 5px;
}
.gold-button::before {
  content: "";
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: -1;
  transform: skew(-15deg);
  border: 1px solid #ffd600;
  border-radius: 4px;
  background: rgba(255, 214, 0, 0.3);
}
</style>