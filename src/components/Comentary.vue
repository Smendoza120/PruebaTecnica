<script setup lang="ts">
import ComentaryInfo from "./component/ComentaryInfo.vue";
import { defineProps as definePropsComentary } from "vue";

const components = [
  {
    image: "../src/components/images/avatar-anisha.png",
    name: "Anisha Li",
    comentary: `“Manage has supercharged our team’s workflow. The ability to maintain 
  visibility on larger milestones at all times keeps everyone motivated.”`,
  },
  {
    image: "../src/components/images/avatar-ali.png",
    name: "Ali Bravo",
    comentary: `“We have been able to cancel so many other subscriptions since using 
  Manage. There is no more cross-channel confusion and everyone is much 
  more focused.”`,
  },
  {
    image: "../src/components/images/avatar-richard.png",
    name: "Richard Watts",
    comentary: `“Manage allows us to provide structure and process. It keeps us organized 
  and focused. I can’t stop recommending them to everyone I talk to!”`,
  },
  {
    image: "../src/components/images/avatar-shanai.png",
    name: "Shanai Gough",
    comentary: `“Their software allows us to track, manage and collaborate on our projects 
  from anywhere. It keeps the whole team in-sync without being intrusive.”`,
  },
];
</script>

<template>
  <section class="comentary__container">
    <div class="comentary__container-info">
      <h3 class="comentary__title">What they’ve said</h3>
      <div class="comentary__flex">
        <ComentaryInfo
          v-for="component in components"
          :image="component.image"
          :name="component.name"
          :comentary="component.comentary"
        />
      </div>
      <button class="comentary__button">Get Started</button>
    </div>

    <div class="comentary__footer">
      <h3 class="comentary__sub-title">Simplify how your team works today.</h3>
      <button class="comentary__button-secundary">Get Started</button>
    </div>
  </section>
</template>

<style>
.comentary__container-info {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  font-family: var(--font-family);
}
.comentary__title {
  text-align: center;
  color: var(--Dark_Blue);
  font-size: 1.8rem;
}
.comentary__flex {
  width: 75%;
  display: flex;
  flex-wrap: nowrap;
  overflow: auto;
}
.comentary__button {
  margin-top: 15px;
  padding: 10px 30px;
  border: none;
  border-radius: 20px;
  background: var(--Bright_Red);
  color: var(--Vary_Light_Gray);
  transition: 0.3s linear;
}

.comentary__button:hover {
  cursor: pointer;
  background: var(--Bright_Red_hover);
}

.comentary__footer {
  width: 100%;
  height: 270px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  background: var(--Bright_Red);
  font-family: var(--font-family);
  padding: 5px;
  margin-top: 30px;
}

.comentary__sub-title {
  font-size: 2.5rem;
  text-align: center;
  margin-bottom: 10px;
  color: white;
  font-weight: 500;
}

.comentary__button-secundary {
  padding: 10px 30px;
  border: none;
  border-radius: 20px;
  background: var(--Vary_Light_Gray);
  color: var(--Bright_Red);
  transition: 0.3s linear;
}

.comentary__button-secundary:hover{
  cursor: pointer;
  opacity:.8;
}
</style>
