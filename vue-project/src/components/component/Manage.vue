<script setup lang="ts">
import { defineProps as fefinePropsManage } from "vue";

const props = defineProps({
  number: {
    type: String,
    required: true,
  },
  title: {
    type: String,
    required: true,
  },
  text: {
    type: String,
    required: true,
  },
});

const { number, title, text } = props;
</script>

<template>
  <section class="manage__container">
    <div class="manage__title-container">
      <div class="manage__number">{{ number }}</div>
      <h4 class="manage__title">{{ title }}</h4>
    </div>
    <p class="manage__text">{{ text }}</p>
  </section>
</template>

<style>
.manage__container {
  font-family: var(--font-family);
}
.manage__title-container {
  display: flex;
  align-items: center;
  gap: 10px;
}
.manage__number{
  background-color: var(--Bright_Red);
  color: white;
  padding: 10px 23px;
  border-radius: 40px;
  font-family: var(--font-family);
}
.manage__title{
  color: var(--Dark_Blue);
  font-weight: 500;
  font-size: 1rem;
}
.manage__text{
  color: var(--Dark_Grayish_Blue);
}
</style>
