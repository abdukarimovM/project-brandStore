<template>
  <header>
    <div class="container mx-auto">
      <nav class="h-[86px] flex items-center justify-between mt-[22px] mb-[10px]">
        <div class="flex items-center">
          <div
            class="flex items-center absolute bg-[#0D6EFD] w-[47px] h-[50px] rounded-[8px]"
          >
            <img
              class="w-[25px] h-[29px] ml-[10px]"
              src="../public/icons/logo.png"
              alt=""
            />
          </div>
          <img class="ml-[12px] h-[50px]" src="../public/icons/2.png" alt="" />
          <img
            class="w-[110px] h-[32px] ml-[10px]"
            src="../public/icons/brand.png"
            alt=""
          />
        </div>
        <!-- search -->
        <div
          class="justify-end flex w-[700px] border border-[#0D6EFD] border-2 rounded-[5px] h-[45px] flex items-center"
        >
          <input class="w-[410px] h-full outline-none" type="text" placeholder="Search" />
          <button
            class="pl-[6px] flex w-[150px] items-center gap-[20px] h-[45px] border border-[#0D6EFD]"
          >
            All category <img src="../public/icons/str.png" alt="" />
          </button>
          <button class="bg-[#127FFF] text-white text-[18px] w-[110px] h-[45px]">
            Search
          </button>
        </div>
        <div class="flex gap-[22px] text-[#8B96A5]">
          <div class="flex flex-col items-center">
            <img
              class="w-[25px] h-[25px] mb-[7px]"
              src="../public/icons/man.svg"
              alt=""
            />
            <p>Profile</p>
          </div>
          <div class="flex flex-col items-center">
            <img
              class="w-[25px] h-[25px] mb-[7px]"
              src="../public/icons/message.svg"
              alt=""
            />
            <p>Message</p>
          </div>
          <div class="flex flex-col items-center">
            <img
              class="w-[25px] h-[25px] mb-[7px]"
              src="../public/icons/yurak.svg"
              alt=""
            />
            <p>Orders</p>
          </div>
          <div class="flex flex-col items-center">
            <img
              class="w-[25px] h-[25px] mb-[7px]"
              src="../public/icons/card.svg"
              alt=""
            />
            <p>My cart</p>
          </div>
        </div>
      </nav>
    </div>
  </header>
</template>

<script setup></script>

<style lang="css" scoped></style>
