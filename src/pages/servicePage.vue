<template>
  <div class="bg-black">
    <section>
      <nav class="z-40 mx-4 md:mx-20 fixed top-0 left-0 w-full py-6 text-white">
        <div class="row">
          <div class="col-2 col-md-8">
            <img
              src="~assets/package.png"
              class="h-8 animate-bounce text-bold"
            />
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
    </section>
    <section>
      <div class="bg-black">
        <q-parallax :height="200" :speed="0.5">
          <template v-slot:media>
            <img
              src="https://blog-media.byjusfutureschool.com/bfs-blog/2022/08/18080907/c-language.png"
            />
          </template>
        </q-parallax>
      </div>
      <div
        class="text-lg md:text-3xl text-bold text-yellow-400 text-center py-3 md:py-10"
      >
        My Programming Skills on
      </div>
      <section
        class="row md:py-10 mt-5 md:mt-0 md:px-20 bg-slate-950 flex gap-3 md:gap-0"
      >
        <div class="col-12 col-md-3 text-center px-2 animate-pulse">
          <q-img
            class="h-[200px] md:h-[400px] w-full rounded-3xl"
            src="  https://blog.logrocket.com/wp-content/uploads/2021/09/ultimate-guide-SVGs-vue-js.png"
          >
            <div class="absolute-bottom text-subtitle1 text-center text-2xl">
              Vue Js
            </div>
          </q-img>
        </div>
        <div class="col-12 col-md-3 text-center px-2 animate-pulse">
          <q-img
            class="h-[200px] md:h-[400px] w-full rounded-3xl"
            src=" data:image/png;base64,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"
          >
            <div class="absolute-bottom text-subtitle1 text-center text-2xl">
              Quasar
            </div>
          </q-img>
        </div>
        <div class="col-12 col-md-3 text-center px-2 animate-pulse">
          <q-img
            class="h-[200px] md:h-[400px] w-full rounded-3xl"
            src=" https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ-N49mFZ-LuXudZi_9oS8FNvm66O0fTrOYsWVUThNcgd8rgUBm7oauTJ-ShH4a6r6_drU&usqp=CAU"
          >
            <div class="absolute-bottom text-subtitle1 text-center text-2xl">
              Java Script
            </div>
          </q-img>
        </div>
        <div class="col-12 col-md-3 text-center px-2 animate-pulse">
          <q-img
            class="h-[200px] md:h-[400px] w-full rounded-3xl"
            src=" data:image/png;base64,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"
          >
            <div class="absolute-bottom text-subtitle1 text-center text-2xl">
              Tailwind
            </div>
          </q-img>
        </div>
      </section>
    </section>
    <section>
      <div
        class="w-full h-32 md:h-96 bg-no-repeat bg-cover bg-center"
        style="
          background-image: url('https://images4.alphacoders.com/130/1307940.png');
        "
      >
        <div class="px-96 pt-40 text-center">
          <div class="text-5xl text-yellow-400 py-5"></div>
        </div>
      </div>
    </section>

    <div
      class="text-1 items-center text-center bg-slate-950 text-yellow-500 pt-8 md:pt-24 text-lg md:text-[65px] font-serif"
    >
      Some of my work & live project here
      <br />

      <q-img
        class="bg-yellow-500 animate-bounce my-5 w-[40px] rounded-3xl"
        src="https://cdn-icons-png.flaticon.com/512/54/54572.png"
      />
    </div>

    <section>
      <div
        class="flex min-h-screen items-center justify-center bg-slate-950 pb-10"
      >
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-5">
          <div
            class="border-2 border-yellow-500 group relative cursor-pointer items-center justify-center overflow-hidden transition-shadow hover:shadow-xl hover:shadow-black/30"
          >
            <div class="h-[450px] w-[450px]">
              <img
                class="h-full w-full object-cover transition-transform duration-500 group-hover:rotate-3 group-hover:scale-125"
                src="~assets/e-commerce.png"
                alt=""
              />
            </div>
            <div
              class="absolute inset-0 bg-gradient-to-b from-transparent via-transparent to-black group-hover:from-black/70 group-hover:via-black/60 group-hover:to-black/70"
            ></div>
            <div
              class="absolute inset-0 flex translate-y-[50%] flex-col items-center justify-center px-9 text-center transition-all duration-500 group-hover:translate-y-0"
            >
              <h1 class="font-dmserif text-3xl font-bold text-white">
                E-commerce Website
              </h1>
              <p
                class="mb-3 text-lg italic text-white opacity-0 transition-opacity duration-300 group-hover:opacity-100"
              >
                Here you can see a
                <span class="text-teal-400 text-bold">E-commerce Website</span>
                design
              </p>
              <q-btn
                href=" https://ecommercewebsitedesign.netlify.app/"
                rounded
                label="Live Project"
                class="py-2 px-5 font-com text-sm bg-teal-950 hover:text-teal-200 text-white capitalize shadow shadow-black/60"
              />
            </div>
          </div>
          <div
            class="group relative cursor-pointer items-center justify-center overflow-hidden transition-shadow hover:shadow-xl hover:shadow-black/30"
          >
            <div class="h-[450px] w-[450px]">
              <img
                class="h-full w-full object-cover transition-transform duration-500 group-hover:rotate-3 group-hover:scale-125"
                src="https://marketplace.canva.com/EAFf9pTh3kg/1/0/566w/canva-black-and-white-simple-portfolio-cover-page-WU-vstmgXMU.jpg"
                alt=""
              />
            </div>
            <div
              class="absolute inset-0 bg-gradient-to-b from-transparent via-transparent to-black group-hover:from-black/70 group-hover:via-black/60 group-hover:to-black/70"
            ></div>
            <div
              class="absolute inset-0 flex translate-y-[50%] flex-col items-center justify-center px-9 text-center transition-all duration-500 group-hover:translate-y-0"
            >
              <h1 class="font-dmserif text-3xl font-bold text-white">
                My portfolio
              </h1>
              <p
                class="mb-3 text-lg italic text-white opacity-0 transition-opacity duration-300 group-hover:opacity-100"
              >
                Here you can see my
                <span class="text-teal-400 text-bold">Portfolio</span> Design.
              </p>
              <q-btn
                href="https://zihadulislam45.netlify.app/#/"
                rounded
                label="Live Project"
                class="py-2 px-5 font-com text-sm bg-teal-950 hover:text-teal-200 text-white capitalize shadow shadow-black/60"
              />
            </div>
          </div>
          <div
            class="group relative cursor-pointer items-center justify-center overflow-hidden transition-shadow hover:shadow-xl hover:shadow-black/30"
          >
            <div class="h-[450px] w-[450px]">
              <img
                class="h-full w-full object-cover transition-transform duration-500 group-hover:rotate-3 group-hover:scale-125"
                src="~assets/cover.png"
                alt=""
              />
            </div>
            <div
              class="absolute inset-0 bg-gradient-to-b from-transparent via-transparent to-black group-hover:from-black/70 group-hover:via-black/60 group-hover:to-black/70"
            ></div>
            <div
              class="absolute inset-0 flex translate-y-[50%] flex-col items-center justify-center px-9 text-center transition-all duration-500 group-hover:translate-y-0"
            >
              <h1 class="font-dmserif text-3xl font-bold text-white">
                Company Website
              </h1>
              <p
                class="mb-3 text-lg italic text-white opacity-0 transition-opacity duration-300 group-hover:opacity-100"
              >
                Here you can see a
                <span class="text-teal-400 text-bold"
                  >Company basic Website</span
                >
                design
              </p>
              <q-btn
                href="https://unrivaled-gecko-4fd94c.netlify.app/#/"
                rounded
                label="Live Project"
                class="py-2 px-5 font-com text-sm bg-teal-950 hover:text-teal-200 text-white capitalize shadow shadow-black/60"
              />
            </div>
          </div>
          <div
            class="group relative cursor-pointer items-center justify-center overflow-hidden transition-shadow hover:shadow-xl hover:shadow-black/30"
          >
            <div class="h-[450px] w-[450px]">
              <img
                class="h-full w-full object-cover transition-transform duration-500 group-hover:rotate-3 group-hover:scale-125"
                src="~assets/now.png"
                alt=""
              />
            </div>
            <div
              class="absolute inset-0 bg-gradient-to-b from-transparent via-transparent to-black group-hover:from-black/70 group-hover:via-black/60 group-hover:to-black/70"
            ></div>
            <div
              class="absolute inset-0 flex translate-y-[50%] flex-col items-center justify-center px-9 text-center transition-all duration-500 group-hover:translate-y-0"
            >
              <h1 class="font-dmserif text-3xl font-bold text-white">
                BPL website
              </h1>
              <p
                class="mb-3 text-lg italic text-white opacity-0 transition-opacity duration-300 group-hover:opacity-100"
              >
                Here you can see a
                <span class="text-teal-400 text-bold"
                  >Cricket tournament website</span
                >
                design
              </p>
              <q-btn
                href="https://bsti-premier-league.netlify.app/#/"
                rounded
                label="Live Project"
                class="py-2 px-5 font-com text-sm bg-teal-950 hover:text-teal-200 text-white capitalize shadow shadow-black/60"
              />
            </div>
          </div>
          <div
            class="group relative cursor-pointer items-center justify-center overflow-hidden transition-shadow hover:shadow-xl hover:shadow-black/30"
          >
            <div class="h-[450px] w-[450px]">
              <img
                class="h-full w-full object-cover transition-transform duration-500 group-hover:rotate-3 group-hover:scale-125"
                src="~assets/pandu.png"
                alt=""
              />
            </div>
            <div
              class="absolute inset-0 bg-gradient-to-b from-transparent via-transparent to-black group-hover:from-black/70 group-hover:via-black/60 group-hover:to-black/70"
            ></div>
            <div
              class="absolute inset-0 flex translate-y-[50%] flex-col items-center justify-center px-9 text-center transition-all duration-500 group-hover:translate-y-0"
            >
              <h1 class="font-dmserif text-3xl font-bold text-white">
                Company Website
              </h1>
              <p
                class="mb-3 text-lg italic text-white opacity-0 transition-opacity duration-300 group-hover:opacity-100"
              >
                Here you can see a
                <span class="text-teal-400 text-bold"
                  >MovingPanda Login Page</span
                >
                design
              </p>
              <q-btn
                href="https://pandalog.netlify.app/"
                rounded
                label="Live Project"
                class="py-2 px-5 font-com text-sm bg-teal-950 hover:text-teal-200 text-white capitalize shadow shadow-black/60"
              />
            </div>
          </div>
          <div
            class="group relative cursor-pointer items-center justify-center overflow-hidden transition-shadow hover:shadow-xl hover:shadow-black/30"
          >
            <div class="h-[450px] w-[450px]">
              <img
                class="h-full w-full object-cover transition-transform duration-500 group-hover:rotate-3 group-hover:scale-125"
                src="~assets/dash.png"
                alt=""
              />
            </div>
            <div
              class="absolute inset-0 bg-gradient-to-b from-transparent via-transparent to-black group-hover:from-black/70 group-hover:via-black/60 group-hover:to-black/70"
            ></div>
            <div
              class="absolute inset-0 flex translate-y-[50%] flex-col items-center justify-center px-9 text-center transition-all duration-500 group-hover:translate-y-0"
            >
              <h1 class="font-dmserif text-3xl font-bold text-white">
                Company Website
              </h1>
              <p
                class="mb-3 text-lg italic text-white opacity-0 transition-opacity duration-300 group-hover:opacity-100"
              >
                Here you can see a
                <span class="text-teal-400 text-bold">DashBoard</span>
                design
              </p>
              <q-btn
                href="https://hilarious-mousse-0835a6.netlify.app/"
                rounded
                label="Live Project"
                class="py-2 px-5 font-com text-sm bg-teal-950 hover:text-teal-200 text-white capitalize shadow shadow-black/60"
              />
            </div>
          </div>
        </div>
      </div>
    </section>

    <section>
      <div class="text-center text-lg bg-teal-950 text-slate-100 py-6">
        Copyright © 2023 Advance Safety Engineering | Powered by Advance Safety
        Engineering
      </div>
    </section>
  </div>
</template>

<script>
import { defineComponent } from "vue";
import { Animate, initTE } from "tw-elements";

initTE({ Animate });
import "animate.css";

export default defineComponent({
  name: "servicePage",
});
</script>
<style>
@import "tailwindcss/base";
@import "tailwindcss/components";
@import "tailwindcss/utilities";
</style>
