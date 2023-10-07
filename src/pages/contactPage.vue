<template>
  <nav class="z-40 fixed top-0 left-0 w-full py-6">
    <div class="container mx-auto flex justify-between">
      <div class="col-8">
        <img src="~assets/package.png" class="h-8 animate-bounce text-bold" />
      </div>
      <div class="col-4 flex">
        <div class="flex gap-10">
          <div class="cursor-pointer text-yellow-500">
            <q-btn class="text-lg" flat to="/">Home</q-btn>
          </div>

          <div class="cursor-pointer text-yellow-500">
            <q-btn class="text-lg" flat to="/service">Service</q-btn>
          </div>
          <div class="cursor-pointer text-yellow-500">
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
  <div class="bg-slate-950 text-white">
    <section>
      <div class="row py-[-50px] md:py-20 px-2 md:px-36">
        <div class="col-12 col-md-4 mx-2 md:mx-7">
          <div class="text-[60px] py-10 animate-pulse text-yellow-500">
            Get in Touch
          </div>
          <div class="row flex">
            <div class="col-4 col-md-12">
              <q-img
                class="border-2 items-center border-yellow-500 w-32 md:w-[200px] rounded-[300px]"
                src="~assets/p.jpg"
              />
            </div>
          </div>
          <div class="py-4">
            <div class="py-3 text-2xl text-yellow-500">Numbers</div>
            <div class="flex text-xl">
              <q-icon
                class="pt-1 pr-4 animate-bounce text-red-500"
                name="call"
              />
              <p>General : 01749470282</p>
            </div>
          </div>

          <div class="py-4">
            <div class="py-3 text-2xl text-yellow-500">Email</div>
            <div class="flex text-xl">
              <q-icon
                class="pt-1 pr-4 animate-bounce text-yellow-300"
                name="email"
              />
              <p>z.i.nayeem45@gmail.com</p>
            </div>
          </div>

          <div class="py-4">
            <div class="py-3 text-2xl text-yellow-500">Free Hour</div>
            <div class="flex text-xl">
              <q-icon
                class="pt-1 pr-4 animate-bounce text-teal-500"
                name="watch"
              />
              <p>Monday — Friday 9am – 5pm</p>
            </div>
          </div>
        </div>
        <div class="col-12 col-md-6 md:mx-7 md:py-20">
          <form class="py-8 bg-white rounded-xl">
            <div class="text-2xl text-gray-950 text-bold py-5 text-center">
              Send me a Message
            </div>
            <div class="px-5 md:px-20 py-10">
              <q-input
                color="secondary"
                class="py-2 border-4"
                rounded
                outlined
                v-model="text"
                label=" Name"
              />
              <q-input
                color="secondary"
                class="py-2"
                rounded
                outlined
                v-model="text"
                label="Phone number"
              />
              <q-input
                color="secondary"
                class="py-2"
                rounded
                outlined
                v-model="text"
                label="Email"
              />
              <q-input
                class="py-3"
                v-model="textareaModel"
                filled
                clearable
                type="textarea"
                color="secondary"
                label="Massege"
                :shadow-text="textareaShadowText"
                @keydown="processTextareaFill"
                @focus="processTextareaFill"
              />
              <q-btn
                to=""
                class="mx-3 px-16 py-3 text-lg"
                no-caps
                outline
                color="primary"
                label="Submit"
              />
            </div>
          </form>
        </div>
      </div>
    </section>

    <section>
      <div class="mx-3 md:mx-36 py-16">
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3651.023519611964!2d90.39924681385392!3d23.782176793481053!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3755c76db868adf1%3A0xf459889a1357ede!2sBSTI%20Quarters!5e0!3m2!1sen!2sbd!4v1675079462877!5m2!1sen!2sbd"
          height="600"
          class="w-full"
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"
        ></iframe>
      </div>
    </section>
    <section>
      <aboutUs />
    </section>
    <q-separator />
    <section>
      <div class="text-center text-lg bg-teal-950 text-slate-100 py-6">
        Copyright © 2023 Advance Safety Engineering | Powered by Advance Safety
        Engineering
      </div>
    </section>
  </div>
</template>

<script>
export default {};
</script>
<style>
@import "tailwindcss/base";
@import "tailwindcss/components";
@import "tailwindcss/utilities";
</style>
