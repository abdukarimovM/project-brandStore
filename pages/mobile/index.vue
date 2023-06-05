<template>
  <section class="bg-[#eff6ff] h-full">
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
        <div class="w-[400px]">
          <Sidebar />
        </div>
        <div class="ml-[30px] w-full">
          <!-- ///////// -->
          <div
            class="rounded-[6px] pl-[20px] border bg-white h-[70px] text-[18px] flex justify-between items-center"
          >
            <h1>12,911 items in <strong>Mobile accessory</strong></h1>
            <div class="flex items-center">
              <input
                class="mr-[13px] w-[20px] h-[20px] border border-[3px] rounded-[6px] border-[#DEE2E7]"
                type="checkbox"
              />
              <p>Verified only</p>
              <select
                class="outline-none bg-transparent ml-[20px] mr-[13px] flex items-center justify-between border w-[180px] h-[42px] rounded-[6px] pr-[16px] pl-[10px]"
              >
                <option>Featured</option>
                <option>Featured</option>
                <option>Featured</option>
                <option>Featured</option>
              </select>
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

          <div class="mt-[15px]">
            <div class="flex justify-end gap-5 py-5 mb-[160px]">
              <div
                class="bg-white px-2 py-2 border border-gray-300 rounded-lg text-[18px] w-[150px]"
              >
                <select class="cursor-pointer bg-white outline-none pr-5 text-gray-800">
                  <option>Show 10</option>
                  <option>Show 10</option>
                  <option>Show 10</option>
                </select>
              </div>
              <ul
                class="flex items-center gap-0 border border-gray-300 rounded-lg text-[18px]"
              >
                <li
                  class="px-2 p-1 bg-white hover:bg-gray-100 cursor-pointer border-r rounded-l-lg"
                >
                  <i class="bx bx-chevron-left text-2xl"></i>
                </li>
                <li
                  v-for="i in 3"
                  class="p-2 px-4 bg-white hover:bg-gray-100 cursor-pointer border-r"
                >
                  {{ i }}
                </li>
                <li
                  class="px-2 p-1 bg-white hover:bg-gray-100 cursor-pointer border-r rounded-r-lg"
                >
                  <i class="bx bx-chevron-right text-2xl"></i>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import PhoneLinks from "../../const/phone-filter";
import MobileLinks from "../../const/mobile-2page";
import Mobile2_Links from "../../const/mobile2-2page";
</script>

<style lang="scss" scoped></style>
