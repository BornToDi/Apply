<template>
  <div class="text-gray-100 font-[Poppins]">
    <nav class="z-40 fixed top-0 left-0 w-full py-6">
      <div class="container mx-auto flex justify-between">
        <div class="col-8">
          <img src="~assets/package.png" class="h-8 animate-bounce text-bold" />
        </div>
        <div class="col-4 flex">
          <div class="flex gap-10">
            <div class="cursor-pointer hover:text-sky-400">
              <q-btn class="text-lg" flat to="/">Home</q-btn>
            </div>

            <div class="cursor-pointer hover:text-sky-400">
              <q-btn class="text-lg" flat to="/service">Service</q-btn>
            </div>
            <div class="cursor-pointer hover:text-sky-400">
              <q-btn
                class="text-lg bg-slate-600 px-7 rounded-full tracking-wide py-3 hover:scale-110 duration-300"
                flat
                to="/contact"
                >Contact</q-btn
              >
            </div>
          </div>
        </div>
      </div>
    </nav>
    <section class="bg-slate-900 h-full flex px-[10%] py-[6%]">
      <img
        src="~assets/Ellipse.png"
        class="z-20 animate-ping w-6 absolute right-56 top-1/3"
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
        class="z-20 animate-ping w-6 absolute right-2/6 bottom-20"
      />
      <img
        src="~assets/Ellipse.png"
        class="z-20 animate-ping w-6 absolute right-1/2 top-52"
      />

      <img src="~assets/wave3.png" class="absolute bottom-20 right-36 w-96" />
      <img
        src="~assets/wave.png"
        class="absolute z-20 bottom-0 right-0 w-2/3"
      />
      <img
        src="~assets/wave.png"
        class="absolute z-20 bottom-0 right-0 w-2/3"
      />
      <div class="flex-1">
        <img
          src="~assets/profile.jpg"
          class="w-10/12 h-[600px] rounded-bl-3xl rounded-tr-3xl"
        />
      </div>

      <div class="flex-1 pt-7 font-serif">
        <div class="absolute">
          <h1 class="text-4xl text-left text-yellow-400 leading-normal py-6">
            <span1>Build real</span1> <span1>real</span1> <br />
            <span1>Unique</span1><span1>design</span1> <br />
            <span1>for</span1> <span1>your</span1> <br />
            <span1 class="underline decoration-teal-500">Company</span1>
          </h1>
          <q-btn
            class="bg-teal-800 hover:bg-green-600 px-14 rounded mx-1 animate-pulse tracking-wide py-4 text-lg cursor-pointer text-yellow-400 hover:text-yellow-200 duration-300 font-serif"
            icon="collections_bookmark"
            label="My CV"
            href="https://drive.google.com/file/d/1XmNeMYINNBvpHPUxb78hYlPlVlcqxiPS/view?usp=drive_link"
          >
          </q-btn>
          <q-btn
            class="bg-teal-800 hover:bg-green-600 px-14 rounded mx-1 animate-pulse tracking-wide py-4 text-lg cursor-pointer text-yellow-400 hover:text-yellow-200 duration-300 font-serif"
            icon="collections_bookmark"
            label="My Professional Achievements"
            href="https://drive.google.com/file/d/11SLHg1kHpKnJWCP3hpX-Nspqu0IlyzbS/view?usp=drive_link"
          />
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

* {
  padding: 0;
  margin: 0;
}

body {
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

h1 {
  font-family: "Montserrat Medium";
  max-width: 40ch;
  text-align: center;
  transform: scale(0.94);
  animation: scale 3s forwards cubic-bezier(0.5, 1, 0.89, 1);
}
@keyframes scale {
  100% {
    transform: scale(1);
  }
}

span1 {
  display: inline-block;
  opacity: 0;
  filter: blur(4px);
}

span1:nth-child(1) {
  animation: fade-in 1s 0.1s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

span1:nth-child(2) {
  animation: fade-in 1s 0.2s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

span1:nth-child(3) {
  animation: fade-in 1s 0.3s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

span1:nth-child(4) {
  animation: fade-in 1s 0.4s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

span1:nth-child(5) {
  animation: fade-in 1s 0.5s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

span1:nth-child(6) {
  animation: fade-in 1s 0.6s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

span1:nth-child(7) {
  animation: fade-in 1s 0.7s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

span1:nth-child(8) {
  animation: fade-in 1s 0.8s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

span1:nth-child(9) {
  animation: fade-in 1s 0.9s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

span1:nth-child(10) {
  animation: fade-in 1s 1s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

span1:nth-child(11) {
  animation: fade-in 1s 1.1s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

span1:nth-child(12) {
  animation: fade-in 1s 1.2s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

span1:nth-child(13) {
  animation: fade-in 1s 1.3s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

span1:nth-child(14) {
  animation: fade-in 1s 1.4s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

span1:nth-child(15) {
  animation: fade-in 1s 1.5s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

span1:nth-child(16) {
  animation: fade-in 1s 1.6s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

span1:nth-child(17) {
  animation: fade-in 1s 1.7s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

span1:nth-child(18) {
  animation: fade-in 1s 1.8s forwards cubic-bezier(0.11, 0, 0.5, 0);
}

@keyframes fade-in {
  100% {
    opacity: 1;
    filter: blur(0);
  }
}
</style>
