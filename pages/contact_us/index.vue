<template>
  <div>
    <section class="flex gap-16">
      <img src="@/assets/images/contact_us.png" alt="" />
      <div>
        <h1 class="text-[100px] text-[#0157AC]">Contact Us</h1>
        <form class="mt-[100px]">
          <div class="flex gap-20">
            <div class="w-[400px] text-[32px] space-y-[100px]">
              <div class="relative">
                <input
                  type="text"
                  id="full_name"
                  class="block rounded-t-lg px-2.5 pb-2.5 pt-5 w-full text-lg text-gray-900 border-0 border-b-[3px] border-black appearance-none focus:outline-none focus:ring-0 peer"
                  placeholder=" "
                />
                <label
                  for="full_name"
                  class="absolute text-[#939393] duration-300 transform -translate-y-4 scale-75 top-0 z-10 origin-[0] start-2.5 peer-focus:text-blue-600 peer-placeholder-shown:scale-100 peer-placeholder-shown:translate-y-0 peer-focus:scale-75 peer-focus:-translate-y-4 rtl:peer-focus:translate-x-1/4 rtl:peer-focus:left-auto"
                  >Full name</label
                >
              </div>
              <div class="relative">
                <input
                  type="text"
                  id="phone"
                  class="block rounded-t-lg px-2.5 pb-2.5 pt-5 w-full text-lg text-gray-900 border-0 border-b-[3px] border-black appearance-none focus:outline-none focus:ring-0 peer"
                  placeholder=" "
                />
                <label
                  for="phone"
                  class="absolute text-[#939393] duration-300 transform -translate-y-4 scale-75 top-0 z-10 origin-[0] start-2.5 peer-focus:text-blue-600 peer-placeholder-shown:scale-100 peer-placeholder-shown:translate-y-0 peer-focus:scale-75 peer-focus:-translate-y-4 rtl:peer-focus:translate-x-1/4 rtl:peer-focus:left-auto"
                  >Phone</label
                >
              </div>
              <div class="relative">
                <input
                  type="tel"
                  id="message"
                  class="block rounded-t-lg px-2.5 pb-2.5 pt-5 w-full text-lg text-gray-900 border-0 border-b-[3px] border-black appearance-none focus:outline-none focus:ring-0 peer"
                  placeholder=" "
                />
                <label
                  for="message"
                  class="absolute text-[#939393] duration-300 transform -translate-y-4 scale-75 top-0 z-10 origin-[0] start-2.5 peer-focus:text-blue-600 peer-placeholder-shown:scale-100 peer-placeholder-shown:translate-y-0 peer-focus:scale-75 peer-focus:-translate-y-4 rtl:peer-focus:translate-x-1/4 rtl:peer-focus:left-auto"
                  >Message</label
                >
              </div>
            </div>
            <div>
              <ul class="space-y-[100px] -mt-10">
                <li class="h-[65px]">
                  <h1 class="text-[#00054B] text-[32px] font-bold">Contact</h1>
                  <p class="text-[#00054B] text-[32px]">hi@green.com</p>
                </li>
                <li class="h-[65px]">
                  <h1 class="text-[#00054B] text-[32px] font-bold">Based in</h1>
                  <p class="text-[#00054B] text-[32px]">
                    New York, California, Ohio
                  </p>
                </li>
                <li class="h-[65px] pt-10">
                  <div class="flex items-center gap-2">
                    <img src="@/assets/svg/phone.svg" alt="" />
                    <img src="@/assets/svg/telegram.svg" alt="" />
                    <img src="@/assets/svg/instagram.svg" alt="" />
                    <img src="@/assets/svg/youtube.svg" alt="" />
                  </div>
                </li>
              </ul>
            </div>
          </div>
          <button
            class="bg-[#027DFC] mt-[100px] rounded-full px-40 py-6 text-white text-[24px]"
          >
            Contact Us
          </button>
        </form>
      </div>
    </section>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
