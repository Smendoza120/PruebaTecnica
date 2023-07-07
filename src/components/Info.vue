<script setup lang="ts">
import Manage from "./component/Manage.vue";

const components = [
  {
    number: "01",
    title: "Track company-wide progress",
    text: `See how your day-to-day tasks fit into the wider vision. Go from 
  tracking progress at the milestone level all the way done to the 
  smallest of details. Never lose sight of the bigger picture again.`,
  },
  {
    number: "02",
    title: "Advanced built-in reports",
    text: `Set internal delivery estimates and track progress toward company 
  goals. Our customisable dashboard helps you build out the reports 
  you need to keep key stakeholders informed.`,
  },
  {
    number: "03",
    title: "Everything you need in one place",
    text: `Stop jumping from one service to another to communicate, store files, 
  track tasks and share documents. Manage offers an all-in-one team 
  productivity solution.`,
  },
];
</script>

<template>
  <section class="info__container">
    <section class="info__container-text">
      <div class="info__data">
        <h2 class="info__title">What’s different about Manage?</h2>
        <p class="info__text">
          Manage provides all the functionality your team needs, without the
          complexity. Our software is tailor-made for modern digital product
          teams.
        </p>
      </div>
    </section>

    <Manage
      v-for="component in components"
      :number="component.number"
      :title="component.title"
      :text="component.text"
    />
  </section>
</template>

<style>
.info__container {
  padding: 0 20px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  gap: 10px;
}

.info__container-text {
  margin-top: 40px;

  font-family: var(--font-family);
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}
.info__data {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
}
.info__title {
  text-align: center;
  color: var(--Dark_Blue);
}
.info__text {
  text-align: center;
  color: var(--Dark_Grayish_Blue);
}
</style>
