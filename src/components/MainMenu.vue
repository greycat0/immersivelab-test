<template>
  <div class="-ml-10" v-if="screenWidth > 1150">
    <menu-items />
  </div>
  <a-drawer
    v-else
    id="menu"
    placement="left"
    :visible="open"
    @close="$emit('close')"
    :drawerStyle="{ 'margin-left': '-50px' }"
    :bodyStyle="{ 'margin-top': '30px' }"
    :closable="false"
    width="320"
  >
    <menu-items />
  </a-drawer>
</template>

<script>
import Vue from "vue";
import { Drawer } from "ant-design-vue";
import "ant-design-vue/lib/drawer/style/css";

import MenuItems from "./MenuItems.vue";

Vue.use(Drawer);
export default {
  components: {
    MenuItems,
  },
  props: {
    open: Boolean,
    screenWidth: Number,
  },
};
</script>

<style>
#menu .ant-drawer-content {
  background: transparent;
}
#menu .ant-drawer-content-wrapper {
  box-shadow: none;
}
</style>