<template>
  <div class="hero min-h-screen z-0 relative">
    <div class="hero-overlay w-full backdrop-blur-sm flex">
      <div class="
                  hero-content
                  text-black
                  w-full
                  h-full
                  lg:w-[40%]
                  bg-tertiary
                  backdrop-blur-md
                  bg-base-100
                ">
        <div class="max-w-md text-[#1b4965]">
          <h1 class="mb-5 text-6xl font-bold flex">
            <!-- {{ props.data }} by -->
            <img src="../assets/LogoCityzen.svg" alt="" class="w-auto" />
          </h1>
          <p class="mb-5">
            CITYZEN est eun projet pilote sur l'engagement citoyen, initié
            depuis Juin 2020 par l'Association Zone Verte Menzah en partenariat
            avec IWatch et financé par l'Union Européenne.
            <button>...</button>
          </p>
          <div class="w-full flex justify-center items-center">
            <button class="btn btn-primary">Help us build cityzen</button>
          </div>
        </div>

      </div>
      <div
        class=" hidden bg-cover bg-center w-[60%] bg-fixed  h-full md:flex justify-center  items-center bg-[url('../assets/images/hero.avif')]">
      </div>
    </div>

    <!-- <img src="../assets/white-wave.svg" class="w-full bottom-0 left-0 absolute" /> -->
  </div>
</template>
<script setup lang="ts">
// import { defineProps } from "vue";
const props: any = defineProps({
  data: String,
});
</script>
