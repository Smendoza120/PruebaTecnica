<script setup lang="ts"></script>

<template>
  <nav class="navbar">
    <h1 class="navbar__title">
      <img class="navbar__logo" src="./icons/logo.svg" alt="Logo" />
    </h1>
    <img class="navbar__menu" src="./icons/icon-hamburger.svg" alt="Menu" />
  </nav>
</template>

<style>
.navbar {
  padding: 0 20px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.navbar__title{
  display: flex;
  align-items: center;
  justify-content: center;
}
.navbar__menu {
  cursor: pointer;
}
</style>
