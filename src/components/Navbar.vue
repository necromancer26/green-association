<template>
  <div
    class="navbar bg-transparent fixed z-50  text-white  md:flex"
    :class="{ change_color: scrollPosition > 50 }"
  >
    <div class="flex-1">
      <!-- <a class="btn btn-ghost normal-case text-xl">daisyUI</a> -->
      <img src="../assets/LogoCityzen.svg" alt="logo" class="w-[120px] min-w-[120px] ml-32" />
      <!-- <img src="../assets/LogoZoneVerte.svg" alt="" class="w-auto h-16" /> -->
    </div>
    <div class="flex-none">
      <ul class="menu menu-horizontal p-0">
        <li><a>Home</a></li>
        <li><a>Projects</a></li>
        <li><a>About us</a></li>
        <li><a>What we do</a></li>
        <li><a>Contact</a></li>
      </ul>
    </div>
  </div>
  
</template>

<script lang="ts" >
import { defineComponent } from "vue";
export default defineComponent({
  data() {
    return {
      scrollPosition: null as any,
    };
  },
  methods: {
    updateScroll() {
      this.scrollPosition = window.scrollY;
    },
  },
  mounted() {
    window.addEventListener("scroll", this.updateScroll);
  },
});
</script>

<style scoped>
.change_color {
  /* background-color: #f8f9fa; */
  background-color: hsl(var(--b1) / 0.5);
  color: black;
  --tw-backdrop-blur: blur(24px);
    backdrop-filter: var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);
}
</style>