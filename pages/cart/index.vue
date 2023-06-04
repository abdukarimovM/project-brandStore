<template>
  <main class="bg-[#eff6ff] h-full pt-[30px]">
    <div class="container mx-auto">
      <div class="flex gap-[30px]">
        <!-- ///////// -->
        <div class="w-[1140px]">
          <h1 class="text-[30px] font-semibold">My cart (3)</h1>
          <!-- ////////// -->
          <div
            class="border bg-white rounded-[6px] pl-[30px] pt-[23px] pb-[30px] mt-[20px] pr-[30px]"
          >
            <div class="flex">
              <div
                class="rounded-[6px] flex items-center justify-center w-[150px] h-[150px]"
              >
                <img
                  class="w-[150px] h-[140px]"
                  src="../../public/images/tshirt2.png"
                  alt=""
                />
              </div>
              <div class="ml-[20px] w-full">
                <div class="flex justify-between w-full">
                  <div class="text-[20px]">
                    <h1 class="font-medium">
                      T-shirts with multiple colors, for men and lady
                    </h1>
                    <p class="mt-[30px] text-[#8B96A5]">
                      Size: medium, Color: blue, Material: Plastic <br />
                      Seller: Artel Market
                    </p>
                  </div>
                  <div class="font-medium text-[20px] mr-[30px]">
                    <p class="ml-[86px]">$78.99</p>
                    <select
                      class="outline-none bg-transparent w-[150px] border mt-[20px] h-[45px] rounded-[6px]"
                    >
                      <option>Qty: 9</option>
                      <option>Qty: 9</option>
                      <option>Qty: 9</option>
                      <option>Qty: 9</option>
                    </select>
                  </div>
                </div>
                <div class="mt-[40px] font-medium mb-[20px]">
                  <button
                    class="mr-[10px] text-[#FA3434] text-[17px] shadow-sm rounded-[6px] border w-[100px] h-[40px]"
                  >
                    Remove
                  </button>
                  <button
                    class="text-[#0D6EFD] w-[130px] text-[17px] shadow-sm rounded-[6px] h-[40px] border"
                  >
                    Save for later
                  </button>
                </div>
              </div>
            </div>
            <hr />
            <div class="flex mt-[20px]">
              <div
                class="border rounded-[6px] flex items-center justify-center w-[150px] h-[140px]"
              >
                <img
                  class="w-[150px] h-[140px]"
                  src="../../public/images/sumka2.png"
                  alt=""
                />
              </div>
              <div class="ml-[20px] w-full">
                <div class="flex justify-between w-full">
                  <div class="text-[20px]">
                    <h1 class="font-medium">
                      T-shirts with multiple colors, for men and lady
                    </h1>
                    <p class="mt-[30px] text-[#8B96A5]">
                      Size: medium, Color: blue, Material: Plastic <br />
                      Seller: Artel Market
                    </p>
                  </div>
                  <div class="font-medium text-[20px] mr-[30px]">
                    <p class="ml-[86px]">$39.00</p>
                    <select
                      class="outline-none bg-transparent w-[150px] border mt-[20px] h-[45px] rounded-[6px]"
                    >
                      <option>Qty: 3</option>
                      <option>Qty: 3</option>
                      <option>Qty: 3</option>
                      <option>Qty: 3</option>
                    </select>
                  </div>
                </div>
                <div class="mt-[40px] font-medium mb-[20px]">
                  <button
                    class="mr-[10px] text-[#FA3434] text-[17px] shadow-sm rounded-[6px] border w-[100px] h-[40px]"
                  >
                    Remove
                  </button>
                  <button
                    class="text-[#0D6EFD] w-[130px] text-[17px] shadow-sm rounded-[6px] h-[40px] border w-[]"
                  >
                    Save for later
                  </button>
                </div>
              </div>
            </div>
            <hr />
            <div class="flex mt-[20px]">
              <div
                class="rounded-[6px] flex items-center justify-center w-[150px] h-[150px]"
              >
                <img
                  class="w-[150px] h-[140px]"
                  src="../../public/images/ciroq2.png"
                  alt=""
                />
              </div>
              <div class="ml-[20px] w-full">
                <div class="flex justify-between w-full">
                  <div class="text-[20px]">
                    <h1 class="font-medium">
                      T-shirts with multiple colors, for men and lady
                    </h1>
                    <p class="mt-[30px] text-[#8B96A5]">
                      Size: medium, Color: blue, Material: Plastic <br />
                      Seller: Artel Market
                    </p>
                  </div>
                  <div class="font-medium text-[20px] mr-[30px]">
                    <p class="ml-[76px]">$170.50</p>
                    <select
                      class="outline-none bg-transparent w-[150px] border mt-[20px] h-[45px] rounded-[6px]"
                    >
                      <option>Qty: 1</option>
                      <option>Qty: 1</option>
                      <option>Qty: 1</option>
                      <option>Qty: 1</option>
                    </select>
                  </div>
                </div>
                <div class="mt-[40px] font-medium mb-[20px]">
                  <button
                    class="mr-[10px] text-[#FA3434] text-[17px] shadow-sm rounded-[6px] border w-[100px] h-[40px]"
                  >
                    Remove
                  </button>
                  <button
                    class="text-[#0D6EFD] w-[130px] text-[17px] shadow-sm rounded-[6px] h-[40px] border w-[]"
                  >
                    Save for later
                  </button>
                </div>
              </div>
            </div>
            <hr />
            <div class="flex justify-between mt-[20px]">
              <button
                class="pl-[15px] gap-[20px] text-white bg-[#127FFF] flex items-center text-[18px] rounded-[6px] h-[50px] w-[180px]"
              >
                <NuxtLink to="/" class="flex gap-[20px]">
                  <img src="../../public/icons/back.svg" alt="" />Back to shop
                </NuxtLink>
              </button>
              <button
                class="justify-center flex items-center text-[18px] rounded-[6px] h-[50px] w-[150px] border text-[#0D6EFD]"
              >
                Remove all
              </button>
            </div>
          </div>
          <!-- ///////// -->

          <!-- /////////////// -->
          <div class="flex gap-[60px]">
            <div class="flex mt-[35px]">
              <img class="w-[68px] h-[68px]" src="../../public/images/qulf.png" alt="" />
              <div class="text-[20px] flex flex-col justify-center ml-[15px]">
                <h1 class="text-[#1C1C1C]">Secure payment</h1>
                <p class="text-[#A9ACB0]">Have you ever finally just</p>
              </div>
            </div>
            <div class="flex mt-[30px]">
              <img
                class="w-[68px] h-[68px]"
                src="../../public/images/message2.png"
                alt=""
              />
              <div class="text-[20px] flex flex-col justify-center ml-[15px]">
                <h1 class="text-[#1C1C1C]">Secure payment</h1>
                <p class="text-[#A9ACB0]">Have you ever finally just</p>
              </div>
            </div>
            <div class="flex mt-[30px]">
              <img
                class="w-[68px] h-[68px]"
                src="../../public/images/delivery.png  "
                alt=""
              />
              <div class="text-[20px] flex flex-col justify-center ml-[15px]">
                <h1 class="text-[#1C1C1C]">Secure payment</h1>
                <p class="text-[#A9ACB0]">Have you ever finally just</p>
              </div>
            </div>
          </div>
          <!-- //////////// -->
        </div>
        <!-- ////////// -->
        <div class="w-[370px] mt-[65px]">
          <div class="bg-white border rounded-[6px] pl-[20px]">
            <p class="text-[#505050] text-[18px] mt-[22px]">Have a coupon?</p>
            <div class="h-[50px] text-[18px] w-[320px] flex mb-[25px] mt-[10px]">
              <div class="rounded-l-[6px] border flex items-cetner w-2/3 pl-[10px]">
                <input
                  class="text-[#8B96A5] outline-none"
                  type="text"
                  placeholder="Add coupon"
                />
              </div>
              <button
                class="rounded-r-[6px] border w-full text-[#0D6EFD] flex items-center justify-center"
              >
                Apply
              </button>
            </div>
          </div>
          <div
            class="bg-white border rounded-[6px] pl-[20px] pr-[25px] mt-[15px] pt-[20px]"
          >
            <div class="flex text-[#505050] justify-between text-[18px]">
              <p>Subtotal:</p>
              <p>$1403.97</p>
            </div>
            <div class="mt-[6px] flex text-[#505050] justify-between text-[18px]">
              <p>Discount:</p>
              <p class="text-[#FA3434]">- $60.00</p>
            </div>
            <div
              class="mt-[6px] flex text-[#505050] justify-between text-[18px] mb-[20px]"
            >
              <p>Tax:</p>
              <p class="text-[#00B517]">+ $14.00</p>
            </div>
            <hr />
            <div class="flex justify-between font-medium mt-[20px]">
              <p class="text-[20px]">Total:</p>
              <p class="text-[24px]">$1357.97</p>
            </div>
            <button
              class="mt-[22px] bg-[#00B517] text-white w-full rounded-[8px] h-[65px] text-[22px] font-medium"
            >
              Checkout
            </button>
            <div class="flex gap-[8px] mt-[20px] mb-[20px] justify-center">
              <img
                class="w-[50px] h-[40px]"
                src="../../public/icons/ex-page3.svg"
                alt=""
              />
              <img class="w-[50px] h-[40px]" src="../../public/icons/union.svg" alt="" />
              <img
                class="w-[50px] h-[40px]"
                src="../../public/icons/pay-page3.svg"
                alt=""
              />
              <img
                class="w-[50px] h-[40px]"
                src="../../public/icons/visa-pay.svg"
                alt=""
              />
              <img
                class="w-[50px] h-[40px]"
                src="../../public/icons/apple-pay.svg"
                alt=""
              />
            </div>
          </div>
        </div>
        <!-- ////////// -->
      </div>
      <!--  -->
      <div class="bg-white pl-[30px] pt-[30px] mt-[30px]">
        <h1 class="font-medium text-[24px]">Saved for later</h1>
        <div class="flex gap-[20px]">
          <div class="w-[383px] bg-white rounded-[6px]" v-for="el in SavedLinks">
            <div class="">
              <img
                class="w-[300px] h-[270px] mt-[20px] mb-[25px]"
                :src="`/images/${el.img}`"
                alt=""
              />
            </div>
            <div>
              <h1 class="text-[22px] font-medium">{{ el.price }}</h1>
              <p class="mt-[10px] mb-[18px] text-[#606060] text-[18px] w-[200px]">
                {{ el.desc }}
              </p>
              <button
                class="flex w-[180px] h-[45px] border text-[#0D6EFD] mb-[25px] rounded-[6px] items-center justify-center gap-[14px]"
              >
                <img class="text-[#0D6EFD]" src="../../public/icons/cart2.svg" alt="" />
                Move to cart
              </button>
            </div>
          </div>
        </div>
      </div>
      <!--  -->
      <div class="mt-[30px] w-full pb-[50px]">
        <div class="w-full">
          <img
            class="absolute w-[1538px] h-[170px]"
            src="../../public/images/blue2.png"
            alt=""
          />
          <img
            class="absolute w-[1000px] h-[170px]"
            src="../../public/images/blue1.png"
            alt=""
          />
        </div>
        <div
          class="flex justify-between items-center h-[120px] text-white pt-[20px] mb-[50px]"
        >
          <div class="flex items-center ml-[40px]">
            <h1 class="absolute text-[28px] font-medium">
              Super discount on more than 100 USD
            </h1>
            <p class="absolute mt-[60px] text-[20px] opacity-50">
              Have you ever finally just write dummy info
            </p>
          </div>
          <button
            class="text-[20px] rounded-[6px] relative mr-[50px] bg-[#FF9017] w-[160px] h-[60px] flex items-center justify-center"
          >
            Shop now
          </button>
        </div>
      </div>
      <!--  -->
    </div>
  </main>
</template>

<script setup>
import SavedLinks from "../../const/saved";
definePageMeta({
  layout: "cart",
});
</script>

<style lang="scss" scoped></style>
