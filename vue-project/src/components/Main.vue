<template>
  <section class="main__container">
    <img
      class="main__ilustration"
      src="./icons/illustration-intro.svg"
      alt="grafics"
    />
    <div class="main__info">
      <h2 class="main__title">
        Bring everyone together to build better products.
      </h2>
      <p class="main__text">
        Manage makes it simple for software teams to plan day-to-day tasks while
        keeping the larger team goals in view.
      </p>
      <button class="main__button">Get Started</button>
    </div>
  </section>
</template>

<style>
.main__container {
  padding: 0 10px;
  width: 100%;
  margin-top: 30px;
  font-family: var(--font-family);
  font-size: var(--FontSize);
}

.main__ilustration {
  width: 100%;
}

.main__info{
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  gap: 0;
}

.main__title {
  text-align: center;
  font-size: 2rem;
  color: var(--Dark_Blue);
}

.main__text{
  color: var(--Dark_Grayish_Blue);
  text-align: center;
}

.main__button{
  padding: 10px;
  border: none;
  border-radius: 20px;
  background: var(--Bright_Red);
  color: var(--Vary_Light_Gray);
  transition: .3s linear;
}
.main__button:hover{
  cursor: pointer;
  background: var(--Bright_Red_hover);
}
</style>
