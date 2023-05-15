<template>
  <main class="bg-gradient-to-tr from-white to-blue-100 min-h-screen">
    <Navbar />
    <section class="min-h-screen flex justify-center items-center max-md:px-4">
      <div class="text-center">
        <div class="md:text-4xl text-2xl font-bold">
          <h1>Get Connected to the Best Remote</h1>
          <br />
          <h1 class="-mt-8">Jobs in Your Field</h1>
        </div>
        <p class="text-slate-600 mt-6 md:text-lg">
          Discover a wide range of remote opportunities on our platform take
          control of your career
        </p>
        <div class="flex gap-x-8 mt-7 justify-center">
          <div>
            <a
              href="#"
              class="px-5 py-3 rounded-full bg-blue-700 text-white shadow-lg shadow-blue-200 hover:shadow-none transition-all ease duration-300"
              >Explore Remote Jobs</a
            >
          </div>
          <div>
            <a
              href="#"
              class="px-5 py-3 rounded-full text-blue-700 underline font-semibold"
              >How it works?</a
            >
          </div>
        </div>
      </div>
    </section>
    <div class="md:px-24 px-3 mb-3">
      <p class="text-lg font-semibold">Featured Jobs</p>
    </div>
    <section
      class="md:px-24 px-3 flex justify-center max-md:flex-col items-center gap-x-4 pb-20"
    >
      <div
        class="md:w-1/3 w-full p-4 pb-6 max-md:mb-4 hover:bg-blue-700 hover:text-white transition-all ease duration-300 bg-white shadow rounded group"
      >
        <div class="flex gap-x-4">
          <div class="w-14 h-14 bg-white p-2 rounded">
            <img
              src="./assets/figma.png"
              class="object-cover w-full h-full"
              alt=""
            />
          </div>
          <div>
            <p class="text-xl font-semibold">Front End Developer</p>
            <p class="font-light text-slate-400 group-hover:text-slate-200">
              Figma
            </p>
          </div>
        </div>
        <div class="my-4 mb-12">
          <p class="text-slate-600 group-hover:text-slate-100">
            We are looking for an experienced front-end developer to join our
            team.
          </p>
        </div>
        <div class="flex justify-between items-center">
          <div>
            <button
              type="button"
              class="bg-slate-200 px-4 py-1 rounded-full group-hover:bg-blue-600 group-hover:text-white font-semibold"
            >
              Rust
            </button>
          </div>
          <div>
            <p class="font-semibold">$70,000 - $90,000</p>
          </div>
        </div>
      </div>
      <div
        class="md:w-1/3 w-full p-4 pb-6 max-md:mb-4 hover:bg-blue-700 hover:text-white transition-all ease duration-300 bg-white shadow rounded group"
      >
        <div class="flex gap-x-4">
          <div class="w-14 h-14 bg-white p-2 rounded">
            <img
              src="./assets/facebook.png"
              class="object-cover w-full h-full"
              alt=""
            />
          </div>
          <div>
            <p class="text-xl font-semibold">Data Scientist</p>
            <p class="font-light text-slate-400 group-hover:text-slate-200">
              Facebook
            </p>
          </div>
        </div>
        <div class="my-4 mb-12">
          <p class="text-slate-600 group-hover:text-slate-100">
            We are seeking a data scientist to join our team.
          </p>
        </div>
        <div class="flex justify-between items-center">
          <div>
            <button
              type="button"
              class="bg-slate-200 px-4 py-1 rounded-full group-hover:bg-blue-600 group-hover:text-white font-semibold"
            >
              Python
            </button>
          </div>
          <div>
            <p class="font-semibold">$100,000 - $130,000</p>
          </div>
        </div>
      </div>
      <div
        class="md:w-1/3 w-full p-4 pb-6 max-md:mb-4 hover:bg-blue-700 hover:text-white transition-all ease duration-300 bg-white shadow rounded group"
      >
        <div class="flex gap-x-4">
          <div class="w-14 h-14 bg-white p-2 rounded">
            <img
              src="./assets/github.png"
              class="object-cover w-full h-full"
              alt=""
            />
          </div>
          <div>
            <p class="text-xl font-semibold">Technical Writter</p>
            <p class="font-light text-slate-400 group-hover:text-slate-200">
              Github
            </p>
          </div>
        </div>
        <div class="my-4 mb-12">
          <p class="text-slate-600 group-hover:text-slate-100">
            We are seeking a technical writter to join our team.
          </p>
        </div>
        <div class="flex justify-between items-center">
          <div>
            <button
              type="button"
              class="bg-slate-200 px-4 py-1 rounded-full group-hover:bg-blue-600 group-hover:text-white font-semibold"
            >
              Documentation
            </button>
          </div>
          <div>
            <p class="font-semibold">$60,000 - $80,000</p>
          </div>
        </div>
      </div>
    </section>
    <Footer />
  </main>
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Navbar,
    Footer,
  },
};
</script>

<style>
html {
  scroll-behavior: smooth;
}
</style>
