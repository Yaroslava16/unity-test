<template>
  <div class="header">
    <ul class="header__list">
      <li class="header__logo-mobile">
        <n-link :to="'/'">
          <img
            class="header__logo-mobile-icon"
            src="~/assets/svg/logo-mobile.svg"
        /></n-link>
      </li>
      <li class="header__bell">
        <img class="header__bell-icon" src="~/assets/svg/bell.svg" />
      </li>
      <li class="header__menu">
        <img class="header__menu-icon" src="~/assets/svg/menu.svg" />
      </li>
      <li class="header__downloads">
        <img class="header__downloads-icon" src="~/assets/svg/downloads.svg" />
      </li>
      <li class="header__photo">
        <img class="header__photo-img" src="~/assets/svg/photo.svg" />
      </li>
    </ul>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.header {
  position: absolute;
  top: 0;
  width: 100vw;
  padding: 3.889vw 6.667vw 14.722vw 3.889vw;

  @media screen and (min-width: 1440px) {
    width: auto;
    padding: 2.431vw 0 3.958vw 0;
    right: 11.9vw;
  }
  &__list {
    display: flex;
    justify-content: space-between;
    align-items: center;

    @media screen and (min-width: 1440px) {
      justify-content: flex-end;
    }
    li {
      cursor: pointer;
      &:not(:last-child) {
        @media screen and (min-width: 1440px) {
          margin-right: 4.167vw;
        }
      }
    }
  }
  &__logo-mobile {
    margin-right: 58.056vw;

    @media screen and (min-width: 1440px) {
      display: none;
    }
    &-icon {
      width: 9.722vw;
      height: 10.833vw;
    }
  }
  &__bell {
    margin-right: 10.556vw;
  }
  &__menu {
    @media screen and (min-width: 1440px) {
      display: none;
    }
  }
  &__menu-icon,
  &__bell-icon,
  &__downloads-icon {
    width: 5.556vw;
    height: 5.556vw;

    @media screen and (min-width: 1440px) {
      width: 1.389vw;
      height: 1.389vw;
    }
  }
  &__downloads,
  &__photo {
    @media screen and (max-width: 1439px) {
      display: none;
    }
  }
  &__photo-img {
    width: 3.194vw;
    height: 3.194vw;
  }
}
</style>
