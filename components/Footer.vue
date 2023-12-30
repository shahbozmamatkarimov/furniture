<template>
  <div class="mt-20">
    <section>
      <div data-aos="fade-up"
        class="flex items-center lg:h-[450px] md:h-[350px] sm:h-[250px] h-[200px] bg-[url('@/assets/images/footer.png')] rounded-[20px] bg-cover bg-center"
      >
        <div class="w-[650px] px-10">
          <h1 data-aos="fade-right" class="lg:text-[40px] md:text-[32px] sm:text-[24px] text-[16px] font-bold text-[#0157AC]">
            Choose the best equipment for your home and order from us
          </h1>
          <p data-aos="fade-right" class="md:text-[16px] sm:text-sm text-xs text-black/50 font-bold sm:mt-7 mt-5 sm:mb-10 mb-5">
            Click the button and contact us now
          </p>
          <button data-aos="fade-up"
            class="md:text-[16px] sm:text-sm text-xs h-[40px] bg-[#027DFC] px-8 text-white flex items-center gap-3 rounded-full"
          >
            CONTACT US <img src="@/assets/svg/show_more.svg" alt="" />
          </button>
        </div>
      </div>
    </section>

    <footer class="grid lg:grid-cols-5 md:grid-cols-3 grid-cols-2 mt-20 font-bold">
      <div data-aos="fade-up">
        <router-link data-aos="fade-up" to="/"><img src="/logo.svg" /></router-link>
        <p class="text-black/40 max-w-[220px] mt-3">
          We committed to ensuring digital accessibility for individuals
        </p>
      </div>
      <ul data-aos="fade-left" class="space-y-3 text-black/40">
        <li data-aos="fade-up" class="text-2xl text-black">Support</li>
        <li>Help Videos</li>
        <li>Accessories</li>
        <li>Support</li>
        <li>View Booking</li>
        <li>Features</li>
      </ul>
      <ul data-aos="fade-left" class="space-y-3 text-black/40 md:mt-0 mt-10">
        <li data-aos="fade-up" class="text-2xl text-black">Service</li>
        <li>Payment & Tax</li>
        <li>Accessories</li>
        <li>Support</li>
        <li>View Booking</li>
        <li>Features</li>
      </ul>
      <ul data-aos="fade-right" class="space-y-3 text-black/40 lg:mt-0 mt-10">
        <li data-aos="fade-up" class="text-2xl text-black">About</li>
        <li>About us</li>
        <li>Announcements</li>
        <li>Contact</li>
        <li>News</li>
        <li>Features</li>
      </ul>
      <div data-aos="fade-right" class="lg:mt-0 mt-10">
        <h1 data-aos="fade-up" class="text-2xl">Our Address</h1>
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
