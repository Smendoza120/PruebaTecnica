<template>
  <section class="footer__container">
    <form action="" class="footer__form">
      <input
        class="footer__input"
        type="text"
        placeholder="Updates in your inbox..."
      />
      <input class="footer__button" type="button" value="GO" />
    </form>
    <div class="footer__list-container">
      <ul class="footer__list">
        <a class="footer__list-link" href="#"><li class="footer__list-data">Home</li></a>
        <a class="footer__list-link" href="#"><li class="footer__list-data">Pricing</li></a>
        <a class="footer__list-link" href="#"><li class="footer__list-data">Products</li></a>
        <a class="footer__list-link" href="#"><li class="footer__list-data">About</li></a>
      </ul>
      <ul class="footer__list">
        <a class="footer__list-link" href="#"><li class="footer__list-data">Careers</li></a>
        <a class="footer__list-link" href="#"><li class="footer__list-data">Comunity</li></a>
        <a class="footer__list-link" href="#"><li class="footer__list-data">Privacy Policy</li></a>
      </ul>
    </div>

    <div class="footer__icons">
      <a href="#"
        ><img
          class="footer__icon"
          src="./icons/icon-facebook.svg"
          alt="Facebook"
      /></a>

      <a href="#">
        <img
          class="footer__icon"
          src="./icons/icon-youtube.svg"
          alt="Youtube"
        />
      </a>

      <a href="#">
        <img
          class="footer__icon"
          src="./icons/icon-twitter.svg"
          alt="Twitter"
        />
      </a>
      <a href="#">
        <img
          class="footer__icon"
          src="./icons/icon-pinterest.svg"
          alt="Pinterest"
        />
      </a>

      <a href="#">
        <img
          class="footer__icon"
          src="./icons/icon-instagram.svg"
          alt="Instagram"
        />
      </a>
    </div>
    <img class="footer__logo" src="./icons/logo-wite.svg" alt="Logo" />
    <p class="footer__text">
      Copyright 2023 Harold Sanchez. All Rights Reserved
    </p>
  </section>
</template>

<style>
.footer__container {
  width: 100%;
  height: 450px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
  padding: 20px 0;
  font-family: var(--font-family);
  background-color: var(--Very_Dark_Blue);
  color: var(--Very_Pale_Red);
}

.footer__form {
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 20px;
}

.footer__input {
  border: none;
  padding: 15px;
  border-radius: 20px;
}
.footer__button {
  padding: 15px 25px;
  border-radius: 20px;
  border: none;
  background: var(--Bright_Red);
  color: var(--Very_Pale_Red);
  font-size: 1rem;
  font-weight: 500;
  transition: 0.3s linear;
}
.footer__button:hover {
  cursor: pointer;
  opacity: 0.8;
}

.footer__list-container {
  width: 70%;
  display: flex;
  align-items: start;
  justify-content: space-between;
}

.footer__list {
  list-style: none;
  display: flex;
  flex-direction: column;
  gap: 10px;
}

.footer__list-link{
  text-decoration: none;
  color: var(--Very_Pale_Red);
  transition: 0.3s linear;
}

.footer__list-link:hover{
  text-decoration: underline;
}

.footer__icons {
  width: 80%;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.footer__icon {
  width: 32px;
  cursor: pointer;
  transition: 0.3s linear;
}

.footer__icon:hover {
  transform: scale(1.1);
}

.footer__text {
  font-size: 0.8rem;
  text-align: center;
  color: var(--Dark_Grayish_Blue);
}
</style>
