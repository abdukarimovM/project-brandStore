<template>
  <Header />
  <hr />
  <Header2 />
  <hr />

  <main class="bg-[#eff6ff] h-[5000px]">
    <div class="container mx-auto">
      <!-- ///////////////// -->
      <div class="flex gap-[10px] text-[#8B96A5] text-[20px] pt-[25px]">
        <p>Home</p>
        <img src="../../public/icons/right-v.svg" alt="" />
        <p class="ml-[5px]">Clothings</p>
        <img src="../../public/icons/right-v.svg" alt="" />
        <p class="ml-[5px]">Men's wear</p>
        <img src="../../public/icons/right-v.svg" alt="" />
        <p class="ml-[5px]">Summer clothing</p>
      </div>
      <!-- ///////////////// -->
      <div class="flex mt-[20px] w-full">
        <div class="bg-red-400 w-[400px] h-[100px]"></div>
        <div class="ml-[30px] w-full">
          <!-- ///////// -->
          <div
            class="rounded-[6px] pl-[20px] border bg-white h-[70px] text-[18px] flex justify-between items-center"
          >
            <h1>12,911 items in <strong>Mobile accessory</strong></h1>
            <div class="flex items-center">
              <p
                class="mr-[13px] w-[25px] h-[25px] border border-[3px] rounded-[5px] border-[#BDBDBD]"
              ></p>
              <p>Verified only</p>
              <button
                class="ml-[20px] mr-[13px] flex items-center justify-between border w-[180px] h-[42px] rounded-[6px] pr-[16px] pl-[10px]"
              >
                Featured <img src="../../public/icons/str.png" alt="" />
              </button>
              <p
                class="rounded-l-[6px] bg-[#DEE2E7] flex items-center border justify-center h-[42px] w-[40px]"
              >
                <img
                  class="w-[22px] h-[22px]"
                  src="../../public/icons/page-2-menu.svg"
                  alt=""
                />
              </p>
              <p
                class="rounded-r-[6px] flex items-center border justify-center h-[42px] w-[40px] mr-[13px]"
              >
                <img
                  class="w-[22px] h-[22px]"
                  src="../../public/icons/page-2-menu2.svg"
                  alt=""
                />
              </p>
            </div>
          </div>
          <!-- //////// -->

          <!-- //////// -->
          <div class="flex mt-[25px] gap-[15px]">
            <div v-for="el in PhoneLinks" class="">
              <button
                class="text-[18px] text-[#505050] rounded-[5px] p-[20px] flex items-center justify-center border border-[#0D6EFD] h-[40px]"
              >
                {{ el.name }}
                <img class="ml-[30px] mr-[-10px]" src="../../public/icons/x.svg" alt="" />
              </button>
            </div>
            <p class="text-[18px] flex items-center ml-[20px] text-[#0D6EFD]">
              Clear all filter
            </p>
          </div>
          <!-- //////// -->
          <div class="flex w-full mt-[20px] gap-[30px]">
            <!-- ///// -->
            <div class="w-[810px] flex grid grid-cols-2 gap-[30px]">
              <div class="w-full bg-white rounded-[6px]" v-for="el in MobileLinks">
                <div class="flex justify-center">
                  <img
                    class="w-[240px] h-[240px] mt-[30px] mb-[35px]"
                    :src="`/images/${el.img}`"
                    alt=""
                  />
                </div>
                <hr />
                <div class="flex mt-[20px] justify-between pl-[20px]">
                  <div>
                    <img :src="`/icons/${el.price}`" alt="" />
                    <img class="mt-[12px]" :src="`/icons/${el.rating}`" alt="" />
                  </div>
                  <div
                    class="mr-[20px] w-[50px] h-[50px] border flex items-center justify-center rounded-[6px]"
                  >
                    <img src="../../public/icons/blue-yurak.svg" alt="" />
                  </div>
                </div>
                <p
                  class="mt-[15px] mb-[18pxgap-[30px]] ml-[20px] text-[#606060] text-[18px] w-[200px]"
                >
                  {{ el.desc }}
                </p>
              </div>
            </div>
            <!-- //// -->
            <div class="w-1/3 flex grid grid-cols-1 gap-[30px]">
              <div class="w-[383px] bg-white rounded-[6px]" v-for="el in Mobile2_Links">
                <div class="flex justify-center">
                  <img
                    class="w-[240px] h-[240px] mt-[30px] mb-[35px]"
                    :src="`/images/${el.img}`"
                    alt=""
                  />
                </div>
                <hr />
                <div class="flex mt-[20px] justify-between pl-[20px]">
                  <div>
                    <img :src="`/icons/${el.price}`" alt="" />
                    <img class="mt-[12px]" :src="`/icons/${el.rating}`" alt="" />
                  </div>
                  <div
                    class="mr-[20px] w-[50px] h-[50px] border flex items-center justify-center rounded-[6px]"
                  >
                    <img src="../../public/icons/blue-yurak.svg" alt="" />
                  </div>
                </div>
                <p
                  class="mt-[15px] mb-[18px] ml-[20px] text-[#606060] text-[18px] w-[200px]"
                >
                  {{ el.desc }}
                </p>
              </div>
            </div>
            <!-- //// -->
          </div>
          <!-- ///////////// -->

          <div>
            <div>
              <button></button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </main>
</template>

<script setup>
import PhoneLinks from "../../const/phone-filter";
import MobileLinks from "../../const/mobile-2page";
import Mobile2_Links from "../../const/mobile2-2page";
</script>

<style lang="scss" scoped></style>
