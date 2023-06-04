<template>
  <div class="w-full h-[250px] bg-[#EFF2F4] mt-[50px]">
    <div
      class="container mx-auto w-full h-[250px] flex flex-col items-center justify-center bg-[#EFF2F4]"
    >
      <p class="text-[24px] font-bold">Subscribe on our newsletter</p>
      <p class="text-[20px] text-[#606060]">
        Get daily news on upcoming offers from many suppliers all over the world
      </p>
      <div class="flex gap-3">
        <div class="relative mt-6">
          <input
            type="text"
            placeholder="Email"
            class="placeholder:text-[20px] pl-[52px] pt-3 placeholder:text-gray-400 w-[370px] h-[45px] py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-indigo-500 focus:border-indigo-500"
          />
          <div class="absolute inset-y-0 left-0 pl-3 flex items-center w-14">
            <img class="w-[25px]" src="../public/icons/sms.svg" alt="" />
          </div>
        </div>
        <button
          class="mt-6 w-[155px] h-[45px] bg-[#127FFF] rounded-md text-[20px] text-white"
        >
          Subscribe
        </button>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
