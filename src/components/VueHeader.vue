<template>
  <header class="s-header">
    <div class="row width-sixteen-col">
      <div class="s-header__block">
        <div class="s-header__logo">
          <a class="logo" href="#">
            <!-- <img src="../assets/images/logo.svg" alt="Homepage" /> -->
            Owen
          </a>
        </div>
        <a class="s-header__menu-toggle" href="#0"><span>Menu</span></a>
      </div>
      <nav class="s-header__nav">
        <ul class="s-header__menu-links">
          <li><a href="#">About</a></li>
          <li><a href="#">Services</a></li>
          <li><a href="#">Journal</a></li>
          <li><a href="#">Contact</a></li>
        </ul>
        <div class="s-header__contact">
          <a href="#" class="btn btn--primary s-header__contact-btn"
            >Let's Work Together</a
          >
        </div>
      </nav>
    </div>
  </header>
</template>

<script lang="ts" setup>
</script>

<style lang="scss" scoped>
.s-header {
  position: absolute;
  top: 24px;
  .row {
    align-items: center;
  }
  &__block {
    height: fit-content;
  }
}
</style>