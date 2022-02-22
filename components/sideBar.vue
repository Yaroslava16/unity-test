<template>
  <div class="side-bar">
    <div class="side-bar__upper-block">
      <n-link :to="'/'"
        ><img class="side-bar__logo" src="~/assets/svg/logo.svg" alt="" />
      </n-link>
      <button class="side-bar__btn" type="button"></button>
    </div>
    <ul class="side-bar__nav-list">
      <li>
        <n-link class="side-bar__nav-link" :to="'/'">
          <svg class="side-bar__nav-icon">
            <use href="~/assets/svg/symbol-defs.svg#icon-exchange"></use>
          </svg>
          <p class="side-bar__nav-page">Home</p></n-link
        >
      </li>
      <li>
        <n-link class="side-bar__nav-link" :to="'/'">
          <svg class="side-bar__nav-icon">
            <use href="~/assets/svg/symbol-defs.svg#icon-home"></use>
          </svg>
          <p class="side-bar__nav-page">Exchange</p></n-link
        >
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  props: {
    btn: {},
    mobile: false,
  },
};
</script>

<style lang="scss" scoped>
.side-bar {
  padding: 3.889vw 6.667vw 3.889vw 3.889vw;
  height: 100vh;

  @media screen and (min-width: 1440px) {
    width: 27.222vw;
    padding: 2.222vw 1.944vw 2.222vw 8.472vw;
    border-right: 0.069vw solid #3e3846;
  }
  &__upper-block {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    margin-bottom: 9.722vw;
    @media screen and (min-width: 1440px) {
      margin-bottom: 4.653vw;
    }
  }
  &__logo {
    width: 37.222vw;
    height: 10.833vw;
    cursor: pointer;
    @media screen and (min-width: 1440px) {
      width: 9.306vw;
      height: 2.708vw;
    }
  }
  &__btn {
    width: 5.556vw;
    height: 5.556vw;
    background-image: url(~/assets/svg/cross.svg);
    background-repeat: no-repeat;
    background-size: cover;
    cursor: pointer;
    transform: rotate(0);
    transition: 0.5s;
    @media screen and (min-width: 1440px) {
      width: 1.389vw;
      height: 1.389vw;
      background-image: url(~/assets/svg/menu.svg);
    }
    &:hover,
    &:focus {
      transform: scale(1.5) rotate(180deg);
      @media screen and (min-width: 1440px) {
        transform: scale(1.5) rotate(0);
      }
    }
  }
  &__nav-link {
    display: flex;
    align-items: center;
    width: 67.222vw;
    padding: 5vw 0 5vw 8.333vw;
    cursor: pointer;
    transition: 0.5s;
    @media screen and (min-width: 1440px) {
      width: 16.806vw;
      padding: 1.25vw 2.083vw;
    }
    &:hover,
    &:focus {
      background: #242731;
      border-radius: 3.889vw;
      @media screen and (min-width: 1440px) {
        border-radius: 0.972vw;
      }
      svg {
        fill: #486cf3;
      }
      p {
        color: #486cf3;
      }
    }
  }
  &__nav-icon {
    width: 5.556vw;
    height: 5.556vw;
    margin-right: 5vw;
    fill: #7f7989;
    transition: 0.5s;

    @media screen and (min-width: 1440px) {
      width: 1.389vw;
      height: 1.389vw;
      margin-right: 1.25vw;
    }
  }
  &__nav-page {
    font-family: Inter;
    font-style: normal;
    font-weight: 500;
    font-size: 3.889vw;
    line-height: 6.667vw;
    color: #7f7989;
    transition: 0.5s;

    @media screen and (min-width: 1440px) {
      font-size: 0.972vw;
      line-height: 1.667vw;
    }
  }
}
</style>
