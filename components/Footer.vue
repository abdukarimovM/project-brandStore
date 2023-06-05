<template>
  <footer>
    <div class="container mx-auto hidden 2xl:block">
      <!-- ////// -->
      <div class="mt-[50px] flex mb-[60px]">
        <div class="">
          <img
            class="w-[180px] h-[55px] mb-[20px]"
            src="../public/images/logo-colored.png"
            alt=""
          />
          <p class="text-[18px] text-[#505050]">
            Best information about the company <br />
            gies here but now lorem ipsum is
          </p>
          <div class="flex gap-[15px] mt-[20px] w-[50px] h-[50px]">
            <img src="../public/icons/facebook.svg" alt="" />
            <img src="../public/icons/twitter.svg" alt="" />
            <img src="../public/icons/linkedin.svg" alt="" />
            <img src="../public/icons/instagram.svg" alt="" />
            <img src="../public/icons/youtube.svg" alt="" />
          </div>
        </div>
        <div class="ml-[80px]">
          <div class="text-[18px] font-medium flex gap-[150px] mb-[5px]">
            <h1>About</h1>
            <h1 class="ml-[36px]">Partnership</h1>
            <h1 class="ml-[-8px]">Information</h1>
            <h1 class="ml-[-11px]">For users</h1>
            <h1 class="ml-[10px]">Get app</h1>
          </div>
          <div class="flex">
            <div class="grid grid-cols-4">
              <div
                v-for="el in FooterLinks"
                class="mr-[120px] mt-[10px] text-[18px] text-[#8B96A5]"
              >
                <p>{{ el.name }}</p>
              </div>
            </div>
            <div class="mt-[10px]">
              <img class="w-[150px] h-[50px]" src="../public/images/f-app.png" alt="" />
              <img
                class="w-[150px] h-[50px] mt-[10px]"
                src="../public/images/f-play.png"
                alt=""
              />
            </div>
          </div>
        </div>
      </div>
      <!-- //////// -->
    </div>
    <div class="h-[80px] w-full bg-[#EFF2F4] hidden 2xl:block">
      <div class="container mx-auto">
        <div class="flex items-center h-[80px] w-full justify-between">
          <p class="text-[18px] text-[#606060]">© 2023 Ecommerce.</p>
          <div class="flex items-center">
            <select
              class="border-none h-[50px] bg-[#EFF2F4] w-[130px] py-3 text-black text-[22px] leading-tight focus:outline-none"
              name="select"
              id="select"
            >
              <option value="1">
                🇺🇸English <img class="h-6" src="../public/images/usa.png" alt="" />
              </option>
              <option value="2">🇺🇿Uzbek <img src="" alt="" /></option>
              <option value="3">🇷🇺Russian</option>
              <option value="2">🇨🇳Chinese</option>
            </select>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script setup>
import FooterLinks from "../const/footer";
</script>

<style lang="scss" scoped></style>
