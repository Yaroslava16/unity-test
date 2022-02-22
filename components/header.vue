<template>
  <div class="header">
    <ul class="header__list">
      <li>
        <img src="~/assets/svg/bell.svg" />
      </li>
      <li><img src="~/assets/svg/downloads.svg" /></li>
      <li><img src="~/assets/svg/photo.svg" /></li>
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
  right: 11.9vw;
  padding-top: 2.431vw;
  &__list {
    display: flex;
    justify-content: flex-end;
    align-items: center;
    li {
      cursor: pointer;
      &:not(:last-child) {
        margin-right: 4.167vw;
      }
      @media screen {
        
      }
    }
  }
}
</style>
