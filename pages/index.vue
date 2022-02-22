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
        img: require("~/assets/svg/cross.svg"),
      },
    };
  },
};
</script>
