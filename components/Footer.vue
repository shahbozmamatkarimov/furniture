<template>
  <div class="mt-20">
    <section>
      <div
        class="flex items-center h-[450px] bg-[url('@/assets/images/footer.png')] bg-cover"
      >
        <div class="w-[650px] px-10">
          <h1 class="text-[40px] font-bold text-[#0157AC]">
            Choose the best equipment for your home and order from us
          </h1>
          <p class="text-black/50 font-bold mt-7 mb-10">
            Click the button and contact us now
          </p>
          <button
            class="h-[40px] bg-[#027DFC] px-8 text-white flex items-center gap-3 rounded-full"
          >
            CONTACT US <img src="@/assets/svg/show_more.svg" alt="" />
          </button>
        </div>
      </div>
    </section>

    <footer class="grid grid-cols-5 mt-20 font-bold">
      <div>
        <router-link to="/"><img src="/logo.svg" /></router-link>
        <p class="text-black/40 max-w-[220px] mt-3">
          We committed to ensuring digital accessibility for individuals
        </p>
      </div>
      <ul class="space-y-3 text-black/40">
        <li class="text-2xl text-black">Support</li>
        <li>Help Videos</li>
        <li>Accessories</li>
        <li>Support</li>
        <li>View Booking</li>
        <li>Features</li>
      </ul>
      <ul class="space-y-3 text-black/40">
        <li class="text-2xl text-black">Service</li>
        <li>Payment & Tax</li>
        <li>Accessories</li>
        <li>Support</li>
        <li>View Booking</li>
        <li>Features</li>
      </ul>
      <ul class="space-y-3 text-black/40">
        <li class="text-2xl text-black">About</li>
        <li>About us</li>
        <li>Announcements</li>
        <li>Contact</li>
        <li>News</li>
        <li>Features</li>
      </ul>
      <div>
        <h1 class="text-2xl">Our Address</h1>
        <p class="mt-3 text-black/40 w-[240px]">
          1485 Par Drive, Burbank Street , California, CA
        </p>
        <div class="flex items-center gap-2 mt-6">
          <img src="@/assets/svg/phone.svg" alt="" />
          <img src="@/assets/svg/telegram.svg" alt="" />
          <img src="@/assets/svg/instagram.svg" alt="" />
          <img src="@/assets/svg/youtube.svg" alt="" />
        </div>
      </div>
    </footer>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped></style>
