<script setup>
import RegionLinks from "../const/region";
import DealsLinks from "../const/deals";
import CategoryLinks from "../const/category";
import HomeLinks from "../const/home";
import GadgetsLink from "../const/gadgets";
import RecommendedLinks from "../const/recommend";
</script>

<template>
  <Header />
  <hr />
  <Header2 />
  <hr />

  <main class="bg-[#eff6ff] h-full">
    <div class="container mx-auto pt-[20px]">
      <!-- //////////////////////////////////////////// -->
      <div class="flex bg-white pt-[20px] pb-[20px] gap-[27px] rounded-[6px]">
        <div>
          <div v-for="el in CategoryLinks" class="w-[250px] ml-[14px]">
            <p
              class="pt-[15px] h-[55px] text-[20px] hover:bg-[#E5F1FF] hover:font-bold rounded-[6px] pl-[10px]"
            >
              {{ el.name }}
            </p>
          </div>
        </div>
        <div class="">
          <h1 class="absolute mt-[55px] ml-[50px] text-[33px]">Latest trending</h1>
          <h1 class="absolute mt-[95px] ml-[50px] text-[37px]">
            <b>Electronic items</b>
          </h1>
          <button
            class="absolute mt-[165px] ml-[50px] text-[20px] bg-white rounded-md p-3"
          >
            Learn More
          </button>
          <img class="w-[910px]" src="../public/images/home-images-1.png" alt="" />
        </div>
        <div class="flex flex-col justify-around">
          <div
            class="w-[280px] h-[200px] bg-[#E3F0FF] flex flex-col items-center rounded-[6px]"
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
          <div class="h-[130px] bg-[#F38332] rounded-md flex items-center">
            <p class="text-[20px] ml-[25px] text-white mb-3">
              Get US $10 off <br />with a new <br />supplier
            </p>
          </div>
          <div class="h-[130px] bg-[#55BDC3] rounded-md flex items-center">
            <p class="text-[20px] ml-[25px] text-white mb-3">
              Send quotes with <br />supplier <br />preferences
            </p>
          </div>
        </div>
      </div>
      <!-- //////////////////////////////////////////// -->

      <!-- //////////////////////////////////////////// -->
      <div class="bg-white mt-[30px] pl-[20px] h-[280px] rounded-[6px] flex">
        <div class="w-[300px] mt-[20px]">
          <h1 class="font-bold text-[24px]">Deals and offers</h1>
          <p class="text-[#8B96A5] text-[20px]">Hygiene equipments</p>
          <div class="mt-[20px]">
            <button class="w-[55px] h-[60px] text-white bg-[#606060] rounded-[4px]">
              <p class="font-bold">04</p>
              Days
            </button>
            <button
              class="ml-[6px] mr-[6px] w-[55px] h-[60px] text-white bg-[#606060] rounded-[4px]"
            >
              <p class="font-bold">13</p>
              Hour
            </button>
            <button
              class="mr-[6px] w-[55px] h-[60px] text-white bg-[#606060] rounded-[4px]"
            >
              <p class="font-bold">34</p>
              Min
            </button>
            <button class="w-[55px] h-[60px] text-white bg-[#606060] rounded-[4px]">
              <p class="font-bold">56</p>
              Sec
            </button>
          </div>
        </div>

        <div class="flex">
          <div
            v-for="el in DealsLinks"
            class="w-[249px] border flex flex-col items-center pt-[17px]"
          >
            <img :src="`/images/${el.img}`" alt="" class="w-[151px] h-[141px]" />
            <span class="mt-[20px] text-[18px]">{{ el.title }}</span>
            <button
              class="mt-[9px] bg-[#FFE3E3] text-[#EB001B] w-[75px] h-[40px] rounded-full"
            >
              {{ el.number }}
            </button>
          </div>
        </div>
      </div>
      <!-- //////////////////////////////////////////// -->

      <!-- //////////////////////////////////////////// -->
      <div class="bg-white rounded-[6px] h-[320px] mt-[20px] flex">
        <div class="">
          <div class="absolute mt-[20px] ml-[20px]">
            <h1 class="font-bold text-[24px]">
              Home and <br />
              outdoor
            </h1>
            <button
              class="w-[150px] h-[50px] text-[20px] bg-white rounded-[6px] mt-[20px]"
            >
              Source now
            </button>
          </div>
          <img class="w-[360px] h-full" src="../public/images/gul-katta.png" alt="" />
        </div>
        <div class="flex w-[1175px] grid grid-cols-4">
          <div v-for="el in HomeLinks" class="border relative">
            <div class="mt-[20px] ml-[16px]">
              <span class="text-[18px]">{{ el.title }}</span>
              <p class="text-[#8B96A5] mt-[9px]">
                From <br />
                USD {{ el.price }}
              </p>
            </div>
            <img
              class="absolute bottom-0 right-0 mr-[9px] mb-[9px] w-[100px] h-[90px]"
              :src="`/images/${el.img}`"
              alt=""
            />
          </div>
        </div>
      </div>
      <!-- //////////////////////////////////////////// -->

      <!-- //////////////////////////////////////////// -->
      <div class="bg-white rounded-[6px] h-[320px] mt-[24px] flex">
        <div class="">
          <div class="absolute mt-[20px] ml-[20px]">
            <h1 class="font-bold text-[24px]">
              Consumer <br />
              electronics and <br />
              gadgets
            </h1>
            <button
              class="w-[150px] h-[50px] text-[20px] bg-white rounded-[6px] mt-[20px]"
            >
              Source now
            </button>
          </div>
          <img class="w-[360px] h-full" src="../public/images/tel-and-nik.png" alt="" />
        </div>
        <div class="flex w-[1175px] grid grid-cols-4">
          <div v-for="el in GadgetsLink" class="border relative">
            <div class="mt-[20px] ml-[16px]">
              <span class="text-[18px]">{{ el.title }}</span>
              <p class="text-[#8B96A5] mt-[9px]">
                From <br />
                USD {{ el.price }}
              </p>
            </div>
            <img
              class="absolute bottom-0 right-0 mr-[9px] mb-[9px] w-[100px] h-[90px]"
              :src="`/images/${el.img}`"
              alt=""
            />
          </div>
        </div>
      </div>
      <!-- //////////////////////////////////////////// -->

      <!-- //////////////////////////////////////////// -->
      <div class="bg-white mt-[20px]">
        <div class="absolute text-white mt-[50px] ml-[50px]">
          <h1 class="text-[40px] font-bold">
            An easy way to send <br />
            requests to all suppliers
          </h1>
          <p class="text-[20px] mt-[18px]">
            Lorem ipsum dolor sit amet, consectetur adipisicing <br />
            elit, sed do eiusmod tempor incididunt.
          </p>
        </div>
        <div
          class="absolute ml-[850px] w-[630px] mt-[50px] h-[450px] rounded-[6px] bg-white pt-[30px] pl-[40px]"
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
            class="bg-[#127FFF] text-white w-[170px] text-[20px] h-[50px] mt-[30px] rounded-[6px]"
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
        <div class="flex grid grid-cols-5 gap-[30px] mt-[30px]">
          <div
            v-for="el in RecommendedLinks"
            class="h-[35px] rounded-[6px] border bg-white h-[370px]"
          >
            <div class="flex flex-col items-center mt-[25px]">
              <img class="w-[180px] h-[190px]" :src="`/images/${el.img}`" alt="" />
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
      <div class="mt-[30px]">
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
      <div class="mt-[30px]">
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
    <Footer2 />
    <Footer />
  </main>
</template>

<style scoped></style>
