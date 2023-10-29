<template>
  <div class="text-gray-100 font-[Poppins]">
    <nav class="z-40 mx-4 md:mx-20 fixed top-0 left-0 w-full py-6">
      <div class="row">
        <div class="col-2 col-md-8">
          <img src="~assets/package.png" class="h-8 animate-bounce text-bold" />
        </div>
        <div class="col-10 col-md-4 flex">
          <div class="flex md:gap-10">
            <div class="cursor-pointer hover:text-sky-400">
              <q-btn class="text-lg" flat to="/">Home</q-btn>
            </div>

            <div class="cursor-pointer hover:text-sky-400">
              <q-btn class="text-lg" flat to="/service">Service</q-btn>
            </div>
            <div class="cursor-pointer hover:text-sky-400">
              <q-btn
                class="text-lg mr-3 bg-slate-600 md:px-7 rounded-full tracking-wide md:py-3 hover:scale-110 duration-300"
                flat
                to="/contact"
                >Contact</q-btn
              >
            </div>
          </div>
        </div>
      </div>
    </nav>
    <section class="section">
      <div class="hero flex items-center justify-between">
        <img
          src="~assets/Ellipse.png"
          class="z-20 animate-ping w-6 absolute right-56 top-1/3"
        />
        <img
          src="~assets/Ellipse.png"
          color="orange"
          class="z-40 animate-ping w-6 absolute left-24 top-16"
        />
        <img
          src="~assets/Ellipse.png"
          color="orange"
          class="z-40 animate-ping w-6 absolute left-24 bottom-12"
        />
        <img
          src="~assets/Ellipse.png"
          color="orange"
          class="z-40 animate-ping w-6 absolute right-24 top-8"
        />
        <img
          src="~assets/Ellipse.png"
          class="z-40 animate-ping w-6 absolute right-52 bottom-52"
        />
        <img
          src="~assets/Ellipse.png"
          class="z-20 animate-ping w-6 absolute left-1/3 bottom-1/3"
        />
        <img
          src="~assets/Ellipse.png"
          class="z-20 animate-ping w-6 absolute right-1/3 bottom-1/3"
        />
        <img
          src="~assets/Ellipse.png"
          class="z-20 animate-ping w-6 absolute right-1/2 top-52"
        />
      </div>
      <div class="section__container">
        <div class="content">
          <p class="subtitle text-lg text-white">HELLO</p>
          <h1 class="title text-white">
            I'm <span>Zihadul<br />a</span> Web Developer
          </h1>
          <p class="description text-yellow-400">
            Welcome to my web developer portfolio! I'm Zihadul, a skilled and
            creative web developer with a passion for creating beautiful,
            responsive, and user-friendly websites. I've worked on a variety of
            web projects.
          </p>
          <div class="action__btns">
            <q-btn
              href="https://drive.google.com/file/d/11SLHg1kHpKnJWCP3hpX-Nspqu0IlyzbS/view?usp=drive_link"
              no-caps
              class="hire__me px-6 py-3 text-xl"
              >Professional Achievements</q-btn
            >
            <q-btn
              href="https://drive.google.com/file/d/1XmNeMYINNBvpHPUxb78hYlPlVlcqxiPS/view?usp=drive_link"
              class="hire__me py-3 px-6 text-xl"
            >
              Cv</q-btn
            >
          </div>
        </div>

        <div class="image">
          <img src="~assets/p.jpg" alt="profile" />
        </div>
      </div>
    </section>
  </div>

  <!--service-->
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "IndexPage",
});
</script>
<style>
@import "tailwindcss/base";
@import "tailwindcss/components";
@import "tailwindcss/utilities";

@import url("https://fonts.googleapis.com/css?family=Montserrat&display=swap");

@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap");

:root {
  --primary-color: #a855f7;
  --primary-color-dark: #9333ea;
  --secondary-color: #ca8a04;
  --text-dark: #1f2937;
  --text-light: #6b7280;
  --extra-light: #000000;
  --max-width: 1200px;
}

* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

a {
  text-decoration: none;
}

body {
  font-family: "Poppins", sans-serif;
}

.section {
  background-color: var(--extra-light);
}

.section__container {
  min-height: 100vh;
  max-width: var(--max-width);
  margin: auto;
  padding: 1rem;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 4rem;
}

.content {
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.subtitle {
  letter-spacing: 2px;
  color: var(--text-light);
  font-weight: 600;
  margin-bottom: 0.5rem;
}

.title {
  font-size: 2.5rem;
  font-weight: 400;
  line-height: 3rem;
  color: var(--text-dark);
  margin-bottom: 1rem;
}

.title span {
  font-weight: 600;
}

.description {
  line-height: 1.5rem;
  color: var(--text-light);
  margin-bottom: 2rem;
}

.action__btns {
  display: flex;
  gap: 1rem;
}

.action__btns button {
  font-size: 1rem;
  font-weight: 600;
  letter-spacing: 2px;
  padding: 1rem 2rem;
  outline: none;
  border: 2px solid var(--primary-color);
  border-radius: 10px;
  transition: 0.3s;
  cursor: pointer;
}

.hire__me {
  background-color: var(--primary-color);
  color: #ffffff;
}

.hire__me:hover {
  background-color: var(--primary-color-dark);
}

.portfolio {
  color: var(--primary-color);
}

.portfolio:hover {
  background-color: var(--primary-color-dark);
  color: #ffffff;
}

.image {
  display: grid;
  place-items: center;
}

.image img {
  width: min(50rem, 60%);
  border-radius: 100%;
}

@media (width < 750px) {
  nav .checkbox {
    display: block;
  }

  ul {
    position: absolute;
    width: 100%;
    height: calc(100vh - 85px);
    left: -100%;
    top: 85px;
    background-color: var(--extra-light);
    flex-direction: column;
    justify-content: center;
    gap: 3rem;
  }

  nav #check:checked ~ ul {
    left: 0;
  }

  ul li a {
    font-size: 1.25rem;
  }

  .section__container {
    padding: 10rem 1rem 5rem 1rem;
    text-align: center;
    grid-template-columns: repeat(1, 1fr);
  }

  .image {
    grid-area: 1/1/2/2;
  }

  .action__btns {
    margin: auto;
  }
}
</style>
