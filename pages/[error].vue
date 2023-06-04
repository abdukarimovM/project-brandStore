<script setup>
definePageMeta({
  layout: "error",
});
</script>

<template>
  <main class="bg-[#eff6ff] h-full">
    <div
      class="container mx-auto pb-[700px] h-[450px] flex justify-center items-center pt-[300px]"
    >
      <img
        src="../public/images/error.png"
        class="mt-[300px]"
        width="500"
        height="500"
        alt=""
      />
      <div style="font-family: sans-serif" class="ml-[50px]">
        <h1 class="text-[#47B886] mt-[300px] text-[80px] text-[#47B886] font-semibold">
          404 not found
        </h1>
        <h1 class="text-[#47B886] text-[31px] mb-[17px]">
          Looking something we don't serve?
        </h1>
        <nuxt-link to="/" class="uppercase hover:underline text-[#295040] text-[25px]"
          >back to home</nuxt-link
        >
      </div>
    </div>
  </main>
</template>

<style lang="scss" scoped></style>
