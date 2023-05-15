<template>
  <nav
    class="py-10 fixed top-0 w-full md:px-24 px-5 transition-all ease duration-300"
  >
    <div class="flex justify-between items-center">
      <div>
        <h2 class="font-semibold text-2xl">Jobless</h2>
      </div>
      <div class="flex gap-x-7 items-center nav-items max-md:hidden">
        <span>
          <a
            href="!#"
            class="text-slate-600 hover:font-semibold transition-all ease"
            >Home</a
          >
        </span>
        <span>
          <a
            href="!#"
            class="text-slate-600 hover:font-semibold transition-all ease"
            >Discover</a
          >
        </span>
        <span>
          <a
            href="!#"
            class="text-slate-600 hover:font-semibold transition-all ease"
            >Post a Job</a
          ></span
        >
        <span
          ><a
            href="!#"
            class="text-slate-600 hover:font-semibold transition-all ease"
            >Contact Us</a
          ></span
        >
      </div>
      <div class="flex gap-3 items-center">
        <div>
          <a
            href="!#"
            class="px-3 py-2 border border-slate-300 rounded font-semibold hover:bg-blue-700 hover:text-white transition-all ease duration-300"
            >Sign Up</a
          >
        </div>
        <div
          class="flex flex-col md:hidden gap-y-1 burger-menu cursor-pointer"
          @click="openMenu()"
        >
          <span
            class="w-6 h-1 border-t-2 line1 border-black transition-all ease duration-300"
          ></span>
          <span
            class="w-6 h-1 border-t-2 line2 border-black transition-all ease duration-300"
          ></span>
          <span
            class="w-6 h-1 border-t-2 line3 border-black transition-all ease duration-300"
          ></span>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  name: "navbar-main",
  methods: {
    scrollAnimate() {
      const nav = document.querySelector("nav");
      if (
        document.documentElement.scrollTop > 100 ||
        document.body.scrollTop > 100
      ) {
        nav.classList.add("bg-white");
        nav.classList.remove("py-10");
        nav.classList.add("py-4");
      } else {
        nav.classList.remove("bg-white");
        nav.classList.remove("py-4");
        nav.classList.add("py-10");
      }
    },
    openMenu() {
      const navItems = document.querySelector(".nav-items");
      const line1 = document.querySelector(".line1");
      const line2 = document.querySelector(".line2");
      const line3 = document.querySelector(".line3");
      line1.classList.toggle("rotate-45");
      line1.classList.toggle("translate-y-1");
      line2.classList.toggle("opacity-0");
      line2.classList.toggle("hidden");
      line3.classList.toggle("-rotate-45");
      line3.classList.toggle("-translate-y-1");
      navItems.classList.toggle("max-md:hidden");
    },
  },
  created() {
    window.addEventListener("scroll", this.scrollAnimate);
  },
};
</script>

<style>
@media screen and (max-width: 576px) {
  .nav-items {
    flex-direction: column;
    position: absolute;
    top: 90px;
    right: 50px;
    gap: 1rem;
    padding: 1.5rem 2.5rem;
    backdrop-filter: blur(10px);
    background: rgba(255, 255, 255, 0.4);
    border-radius: 3px;
  }
}
</style>
