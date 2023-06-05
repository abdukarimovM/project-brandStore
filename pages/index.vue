<script setup>
import RegionLinks from "../const/region";
import DealsLinks from "../const/deals";
import CategoryLinks from "../const/category";
import HomeLinks from "../const/home";
import GadgetsLink from "../const/gadgets";
import RecommendedLinks from "../const/recommend";
</script>

<template>
  <section class="bg-[#eff6ff] h-full">
    <div class="container mx-auto 2xl:pt-[20px]">
      <!-- //////////////////////////////////////////// -->
      <div
        class="2xl:flex justify-between bg-white 2xl:pt-[20px] overflow-hidden 2xl:pb-[20px] 2xl:gap-[30px] rounded-[6px] border-gray-300"
      >
        <div
          class="w-full 2xl:w-[300px] grid 2xl:flex auto-cols-max 2xl:flex-col grid-flow-col gap-2 2xl:gap-1 p-5 2xl:p-0 overflow-scroll 2xl:overflow-hidden"
        >
          <div v-for="el in CategoryLinks" class="2xl:w-[280px] 2xl:ml-[14px]">
            <p
              class="flex items-center 2xl:pl-[10px] bg-[#EFF2F4] 2xl:bg-white text-[#0D6EFD] 2xl:text-[#1C1C1C] h-[55px] text-[20px] 2xl:hover:bg-[#E5F1FF] 2xl:hover:font-bold rounded-[6px]"
            >
              {{ el.name }}
            </p>
          </div>
        </div>

        <div class="flex-grow bg-slate-300 relative 2xl:mx-5">
          <div
            class="text-[20px] 2xl:h2 absolute w-full top-8 2xl:top-16 left-6 2xl:left-12"
          >
            <h1 class="text-[20px] 2xl:absolute 2xl:ml-[50px] w-full 2xl:text-[33px]">
              Latest trending
            </h1>
            <h1 class="2xl:absolute 2xl:mt-[60px] 2xl:ml-[50px] 2xl:text-[37px]">
              <b>Electronic items</b>
            </h1>
            <button
              class="text-[#0D6EFD] 2xl:absolute 2xl:mt-[150px] 2xl:ml-[50px] 2xl:ext-[20px] 2xl:bg-white 2xl:rounded-md 2xl:p-3 h6 bg-white px-4 py-3 rounded-lg mt-5"
            >
              Learn More
            </button>
          </div>
          <img
            class="w-full 2xl:h-[527px] h-[200px] object-cover 2xl:w-[1100px]"
            src="../public/images/home-images-1.png"
            alt=""
          />
        </div>
        <div class="hidden 2xl:block flex flex-col justify-around">
          <div
            class="w-[280px] h-[200px] mb-[34px] mr-[20px] bg-[#E3F0FF] flex flex-col items-center rounded-[6px]"
          >
            <div class="flex pt-[16px] gap-[9px] mb-[14px]">
              <img class="w-[60px]" src="../public/icons/home-avatar.svg" alt="" />
              <p class="text-[20px]">Hi, user <br />let's get stated</p>
            </div>
            <button
              class="bg-[#127FFF] text-white w-[240px] h-[45px] rounded-[6px] text-[17px]"
            >
              Join now
            </button>
            <button
              class="mt-[7px] bg-white rounded-[6px] text-[#0D6EFD] w-[240px] h-[45px] border text-[18px]"
            >
              Log in
            </button>
          </div>
          <div
            class="h-[130px] bg-[#F38332] mb-[30px] mr-[20px] rounded-md flex items-center"
          >
            <p class="text-[20px] ml-[25px] text-white mb-3">
              Get US $10 off <br />with a new <br />supplier
            </p>
          </div>
          <div class="h-[130px] bg-[#55BDC3] rounded-md flex mr-[20px] items-center">
            <p class="text-[20px] ml-[25px] text-white mb-3">
              Send quotes with <br />supplier <br />preferences
            </p>
          </div>
        </div>
      </div>
      <!-- //////////////////////////////////////////// -->

      <!-- //////////////////////////////////////////// -->
      <div
        class="bg-white 2xl:mt-[30px] 2xl:pl-[20px] 2xl:h-[280px] overflow-hidden border-gray-300 2xl:flex"
      >
        <div
          class="2xl:w-[300px] 2xl:mt-[20px] px-2 py-5 flex items-center justify-between 2xl:block"
        >
          <div>
            <h1 class="font-bold text-[24px]">Deals and offers</h1>
            <p class="text-[#8B96A5] text-[20px]">Hygiene equipments</p>
          </div>

          <div class="2xl:mt-[20px] mt-5 flex gap-2">
            <div
              class="w-[55px] h-[60px] 2xl:text-white text-[#8B96A5] flex flex-col items-center justify-center bg-[#EFF2F4] 2xl:bg-[#606060] rounded-[4px]"
            >
              <p class="font-bold">04</p>
              Days
            </div>

            <div
              class="2xl:ml-[6px] 2xl:mr-[6px] w-[55px] h-[60px] 2xl:text-white text-[#8B96A5] bg-[#EFF2F4] flex flex-col items-center 2xl:bg-[#606060] justify-center rounded-[4px]"
            >
              <p class="font-bold">13</p>
              Hour
            </div>

            <button
              class="2xl:mr-[6px] w-[55px] h-[60px] 2xl:text-white bg-[#EFF2F4] text-[#8B96A5] rounded-[4px] flex flex-col items-center 2xl:bg-[#606060] justify-center"
            >
              <p class="font-bold">34</p>
              Min
            </button>
            <button
              class="w-[55px] h-[60px] 2xl:text-white bg-[#606060] bg-[#EFF2F4] text-[#8B96A5] rounded-[4px] flex flex-col items-center 2xl:bg-[#606060] justify-center"
            >
              <p class="font-bold">56</p>
              Sec
            </button>
          </div>
        </div>

        <div class="flex overflow-scroll 2xl:overflow-hidden">
          <div
            v-for="el in DealsLinks"
            class="2xl:w-[249px] 2xl:border border-2 border-gray-300 p-5 2xl:flex 2xl:flex-col 2xl:items-center 2xl:pt-[17px]"
          >
            <div class="w-[130px] 2xl:w-auto flex justify-center 2xl:block">
              <img
                :src="`/images/${el.img}`"
                alt=""
                class="2xl:w-[151px] 2xl:h-[141px] w-[100px] h-[100px] object-cover"
              />
            </div>
            <div class="text-center">
              <p class="text-[18px] mt-[10px]">{{ el.title }}</p>
              <button
                class="bg-[#FFE3E3] text-[#EB001B] w-[75px] h-[40px] mt-[10px] rounded-full"
              >
                {{ el.number }}
              </button>
            </div>
          </div>
        </div>
      </div>
      <!-- //////////////////////////////////////////// -->

      <!-- //////////////////////////////////////////// -->
      <h3 class="h3 my-5 px-5 2xl:hidden text-[20px]"><span>Home and outdoor</span></h3>

      <div
        class="bg-white rounded-[6px] 2xl:h-[320px] 2xl:mt-[20px] flex border-2 border-y border-gray-300 overflow-hidden"
      >
        <div class="">
          <div class="2xl:ml-[20px] hidden 2xl:block">
            <h1 class="mt-[30px] 2xl:absolute font-bold text-[24px] 2xl:text-black">
              Home and <br />
              outdoor
            </h1>
            <button
              class="2xl:absolute 2xl:w-[150px] 2xl:h-[50px] text-[20px] bg-white rounded-[6px] 2xl:mt-[120px]"
            >
              Source now
            </button>
          </div>
          <div class="hidden 2xl:block flex-shrink-0 bg-slate-300">
            <img
              class="w-[360px] h-full object-cover"
              src="../public/images/gul-katta.png"
              alt=""
            />
          </div>
        </div>
        <div
          class="flex w-full overflow-scroll 2xl:overflow-hidden 2xl:w-[1175px] 2xl:grid 2xl:grid-cols-4"
        >
          <div v-for="el in HomeLinks" class="border relative border-gray-300 p-5">
            <div
              class="w-[150px] 2xl:w-auto flex justify-center 2xl:block 2xl:absolute 2xl:bottom-3 2xl:right-4 mb-3 2xl:mb-0"
            >
              <img
                class="w-[82px] h-[82px] object-cover"
                :src="`/images/${el.img}`"
                alt=""
              />
            </div>

            <div class="">
              <span class="text-[18px]">{{ el.title }}</span>
              <p class="2xl:text-[#8B96A5] body-mc-muted 2xl:mt-[9px]">
                From <br />
                USD {{ el.price }}
              </p>
            </div>
          </div>
        </div>
      </div>
      <!-- //////////////////////////////////////////// -->
      <button
        class="h6 bg-white mx-3 px-5 py-3 bg-[#eff6ff] mt-[20px] rounded-lg 2xl:hidden flex gap-3 items-center"
      >
        <h6 class="text-[#0D6EFD]">Source now</h6>

        <img src="../public/icons/str-r.svg" alt="" />
      </button>

      <h3 class="text-[24px] my-5 px-5 2xl:hidden"><span>Consumer electronics</span></h3>

      <!-- //////////////////////////////////////////// -->
      <div
        class="bg-white rounded-[6px] 2xl:h-[320px] 2xl:mt-[24px] flex border-2 border-y border-gray-300 overflow-hidden"
      >
        <div class="">
          <div class="hidden 2xl:block flex-shrink-0 bg-slate-300 relative">
            <div class="ml-[20px] hidden 2xl:block">
              <h1 class="2xl:absolute font-bold 2xl:text-[24px] mt-[30px]">
                Consumer <br />
                electronics and <br />
                gadgets
              </h1>
              <button
                class="2xl:absolute 2xl:w-[150px] h-[50px] text-[20px] bg-white rounded-[6px] mt-[160px]"
              >
                Source now
              </button>
            </div>

            <img
              class="w-[360px] h-full object-cover"
              src="../public/images/tel-and-nik.png"
              alt=""
            />
          </div>
        </div>
        <div
          class="flex 2xl:w-[1175px] 2xl:grid 2xl:grid-cols-4 overflow-scroll 2xl:overflow-hidden"
        >
          <div
            v-for="el in GadgetsLink"
            class="2xl:border relative border-gray-300 p-5 border"
          >
            <div
              class="w-[150px] 2xl:w-auto flex justify-center 2xl:block 2xl:absolute 2xl:bottom-3 2xl:right-3 mb-3 2xl:mb-0"
            >
              <img
                class="w-[82px] h-[82px] object-cover"
                :src="`/images/${el.img}`"
                alt=""
              />
            </div>

            <div class="">
              <span class="text-[18px]">{{ el.title }}</span>
              <p class="text-[#8B96A5] mt-[9px] body-mc-muted">
                From <br />
                USD {{ el.price }}
              </p>
            </div>
          </div>
        </div>
      </div>
      <!-- //////////////////////////////////////////// -->

      <button
        class="h6 bg-white mx-3 px-5 py-3 bg-[#eff6ff] mt-[20px] rounded-lg 2xl:hidden flex gap-3 items-center"
      >
        <h6 class="text-[#0D6EFD]">Source now</h6>

        <img src="../public/icons/str-r.svg" alt="" />
      </button>

      <!-- //////////////////////////////////////////// -->
      <div
        class="mt-[40px] bg-white 2xl:mt-[20px] flex border-2 border-gray-300 rounded-lg overflow-hidden"
      >
        <div class="absolute text-white mt-[30px] 2xl:mt-[50px] ml-[50px]">
          <h1 class="2xl:text-[40px] text-[25px] font-bold">
            An easy way to send <br />
            requests to all suppliers
          </h1>
          <p class="text-[20px] mt-[18px] hidden 2xl:block">
            Lorem ipsum dolor sit amet, consectetur adipisicing <br />
            elit, sed do eiusmod tempor incididunt.
          </p>
          <button
            class="bg-[#127FFF] mt-[20px] 2xl:hidden text-white w-[170px] text-[20px] h-[50px] 2xl:mt-[30px] rounded-[6px]"
          >
            Send inquiry
          </button>
        </div>
        <div
          class="2xl:block hidden absolute ml-[850px] w-[630px] mt-[50px] h-[450px] rounded-[6px] bg-white pt-[30px] pl-[40px]"
        >
          <h1 class="text-[24px] font-bold">Send quote to suppliers</h1>
          <p
            class="rounded-[6px] w-[530px] border h-[40px] flex items-center text-[20px] mt-[20px] pl-[15px]"
          >
            What item you need?
          </p>
          <textarea
            class="border w-[530px] mt-[20px] pt-[11px] pl-[11px] text-[18px] rounded-[6px] outline-none"
            placeholder="Type more details"
            name=""
            id=""
            rows="4"
          ></textarea>
          <div class="flex">
            <p
              class="rounded-[6px] mt-[25px] border text-[20px] w-[250px] pl-[12px] flex items-center h-[50px]"
            >
              Quantity
            </p>
            <select
              class="outline-none mt-[25px] bg-transparent rounded-[6px] border text-[20px] w-[100px] focus:border-[#127FFF] ml-[10px] h-[50px]"
            >
              <option>Pcs</option>
              <option>Pcs</option>
              <option>Pcs</option>
              <option>Pcs</option>
            </select>
          </div>
          <button
            class="bg-[#127FFF] text-white w-[170px] text-[20px] h-[50px] 2xl:mt-[30px] rounded-[6px]"
          >
            Send inquiry
          </button>
        </div>
        <img
          class="big-images rounded-[6px]"
          src="../public/images/big-image.png"
          alt=""
        />
      </div>
      <!-- //////////////////////////////////////////// -->

      <!-- //////////////////////////////////////////// -->
      <div class="mt-[25px]">
        <h1 class="text-[28px] font-bold">Recommended items</h1>
        <div
          class="overflow-scroll 2xl:overflow-hidden 2xl: 2xl:flex flex 2xl:grid 2xl:grid-cols-5 grid-cols-2 2xl:gap-[30px] mt-[30px]"
        >
          <div
            v-for="el in RecommendedLinks"
            class="h-[35px] rounded-[6px] border bg-white h-[370px]"
          >
            <div class="overflow-hidden 2xl:flex 2xl:flex-col items-center mt-[25px]">
              <img
                class="object-cover w-[180px] h-[190px]"
                :src="`/images/${el.img}`"
                alt=""
              />
            </div>
            <h1 class="ml-[16px] text-[22px] mt-[30px]">{{ el.price }}</h1>
            <p class="ml-[16px] text-[18px] text-[#8B96A5] mt-[5px] w-[180px]">
              {{ el.desc }}
            </p>
          </div>
        </div>
      </div>
      <!-- //////////////////////////////////////////// -->

      <!-- //////////////////////////////////////////// -->
      <div class="mt-[30px] hidden 2xl:block">
        <h1 class="text-[28px] font-semibold">Our extra services</h1>
        <div class="flex grid grid-cols-4 gap-[25px]">
          <div class="w-[362px] h-[300px] bg-white mt-[24px] rounded-[6px]">
            <img
              class="w-full bg-[#374151] h-[180px] rounded-t-[6px]"
              src="../public/images/firma1.png"
              alt=""
            />
            <p class="text-[20px] mt-[25px] ml-[30px] font-medium">
              Source from <br />
              Industry Hubs
            </p>
            <div
              class="border border-white border-[3px] mt-[-120px] ml-[250px] absolute bg-[#D1E7FF] w-[80px] h-[80px] rounded-full flex justify-center items-center"
            >
              <img class="w-[25px] h-[25px]" src="../public/icons/search.svg" alt="" />
            </div>
          </div>
          <div class="w-[362px] h-[300px] bg-white mt-[24px] rounded-[6px]">
            <img
              class="bg-[#374151] h-[180px] rounded-t-[6px]"
              src="../public/images/kamalak.png"
              alt=""
            />
            <p class="text-[20px] mt-[25px] ml-[30px] font-medium">
              Source from <br />
              Industry Hubs
            </p>
            <div
              class="border border-white border-[3px] mt-[-120px] ml-[250px] absolute bg-[#D1E7FF] w-[80px] h-[80px] rounded-full flex justify-center items-center"
            >
              <img class="w-[25px] h-[25px]" src="../public/icons/kam-icon.svg" alt="" />
            </div>
          </div>
          <div class="w-[362px] h-[300px] bg-white mt-[24px] rounded-[6px]">
            <img
              class="bg-[#374151] h-[180px] rounded-t-[6px]"
              src="../public/images/fly.png"
              alt=""
            />
            <p class="text-[20px] mt-[25px] ml-[30px] font-medium">
              Source from <br />
              Industry Hubs
            </p>
            <div
              class="border border-white border-[3px] mt-[-120px] ml-[250px] absolute bg-[#D1E7FF] w-[80px] h-[80px] rounded-full flex justify-center items-center"
            >
              <img class="w-[25px] h-[25px]" src="../public/icons/sam.svg" alt="" />
            </div>
          </div>
          <div class="w-[362px] h-[300px] bg-white mt-[24px] rounded-[6px]">
            <img
              class="bg-[#374151] h-[180px] rounded-t-[6px]"
              src="../public/images/firma2.png"
              alt=""
            />
            <p class="text-[20px] mt-[25px] ml-[30px] font-medium">
              Source from <br />
              Industry Hubs
            </p>
            <div
              class="border border-white border-[3px] mt-[-120px] ml-[250px] absolute bg-[#D1E7FF] w-[80px] h-[80px] rounded-full flex justify-center items-center"
            >
              <img
                class="w-[25px] h-[25px]"
                src="../public/icons/firma-icon.svg"
                alt=""
              />
            </div>
          </div>
        </div>
      </div>
      <!-- //////////////////////////////////////////// -->

      <!-- //////////////////////////////////////////// -->
      <div class="mt-[30px] pb-[50px] hidden 2xl:block">
        <h1 class="text-[28px] font-semibold">Suppliers by region</h1>
        <div>
          <div class="grid grid-cols-5 mt-[10px]">
            <div class="flex mt-[15px] items-center" v-for="el in RegionLinks">
              <img class="w-[40px] h-[30px]" :src="`/icons/${el.img}`" alt="" />
              <div class="ml-[15px]">
                <h1 class="text-[20px]">{{ el.title }}</h1>
                <p class="text-[#8B96A5] text-[16px]">{{ el.desc }}</p>
              </div>
            </div>
          </div>
          <div></div>
        </div>
      </div>
      <!-- //////////////////////////////////////////// -->
    </div>
  </section>
</template>

<style scoped></style>
