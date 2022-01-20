<template>
  <header class="header">
    <nav class="header__nav">
      <NuxtLink to="#home" class="logo" title="Kariston Stefane">K</NuxtLink>
      <ul class="menu">
        <li class="menu__item">
          <NuxtLink class="menu__link" to="#projects" title="Projects"
            >Projects</NuxtLink
          >
        </li>
        <li class="menu__item">
          <NuxtLink class="menu__link" to="#resume" title="Resume"
            >Resume</NuxtLink
          >
        </li>
        <li class="menu__item">
          <NuxtLink class="menu__link" to="#contact" title="Contact"
            >Contact</NuxtLink
          >
        </li>
      </ul>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
.header {
  position: fixed;
  top: 0;
  z-index: 100;
  width: 100%;
  background-color: rgba($color-bg-alt, 0.5);
  backdrop-filter: blur(50px);
  padding: 1.5rem 0;

  &__nav {
    width: 100%;
    padding: 0 12.5%;

    display: flex;
    gap: 1rem;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
  }

  .logo {
    display: flex;
    align-items: center;
    justify-content: center;

    font: 700 1.5rem $font-title;
    color: $color-primary;
    text-decoration: none;

    width: 3rem;
    height: 3rem;
    border-radius: 100%;
    border: 2px solid $color-primary;
  }

  .menu {
    display: flex;
    align-items: center;
    gap: 1.5rem;
    list-style: none;
    padding: 0;
    margin: 0;

    &__link {
      text-decoration: none;
      font-family: $font-title;
      color: $color-text;
      transition: color 0.3s;

      &.nuxt-link-active {
        color: $color-primary;
      }
    }
  }
}
</style>
