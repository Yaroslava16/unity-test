<template>
  <SideBar :btn="btn" />
</template>

<script>
import SideBar from "~/components/sideBar.vue";
export default {
  name: "IndexPage",
  components: {
    SideBar,
  },
  data() {
    return {
      btn: {
        imgCross: require("~/assets/svg/cross.svg"),
        img: require("~/assets/svg/menu.svg"),
      },
    };
  },
};
</script>
