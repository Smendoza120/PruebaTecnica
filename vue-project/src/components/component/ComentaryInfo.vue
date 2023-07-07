<script setup lang="ts">
import { defineProps as definePropsComentary } from "vue";

const props = defineProps({
  image: {
    type: String,
    required: true,
    validator: (value: string) => {
      const pattern = /\.(jpeg|jpg|gif|png|svg)$/i;
      return pattern.test(value);
    },
  },
  name: {
    type: String,
    required: true,
  },
  comentary: {
    type: String,
    required: true,
  },
});

const { image, name, comentary } = props;
</script>

<template>
  <div class="comentary__carrusel">
    <div class="comentary__info">
      <img class="comentary__image" :src="image" :alt="`image_${name}`" />
      <h4 class="comentary__name">{{ name }}</h4>
      <p class="comentary__text">{{ comentary }}</p>
    </div>
  </div>
</template>

<style>
.comentary__carrusel{
  width: 280px;
  display: flex;
  align-items: start;
  justify-content: flex-start;
  flex-direction: row;
  flex: 0 0 auto;
}
.comentary__info {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  font-family: var(--font-family);
  padding: 10px 0;
}
.comentary__image {
  width: 100px;
}
.comentary__name {
  font-size: 1.3rem;
  color: var(--Dark_Blue);
}
.comentary__text {
  text-align: center;
  color: var(--Dark_Grayish_Blue);
}
</style>
