<template>
  <div>
    <SideBar  />
    <Header />
  </div>
</template>

<script>
import SideBar from "~/components/sideBar.vue";
import Header from "~/components/header.vue";
export default {
  name: "IndexPage",
  components: {
    SideBar,
    Header,
  },
  data() {
    return {};
  },
};
</script>
