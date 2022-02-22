<template>
  <div class="side-bar">
    <div class="side-bar__upper-block">
      <n-link :to="'/'"
        ><img class="side-bar__logo" src="~/assets/svg/logo.svg" alt="" />
      </n-link>
      <button class="side-bar__btn" type="button"><img :src="btn.img" alt=""></button>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    btn: {},
  },
};
</script>

<style lang="scss" scoped>
.side-bar {
  padding: 3.889vw 6.667vw 3.889vw 3.889vw;
  &__upper-block {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    margin-bottom: 9.722vw;
  }
}
</style>
