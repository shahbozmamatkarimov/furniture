<template>
  <Swiper
    class="rounded-[30px] overflow-hidden"
    :modules="[SwiperAutoplay, SwiperEffectCreative]"
    :slides-per-view="1"
    :loop="true"
    :effect="'creative'"
    spaceBetween="30"
    :centeredSlides="true"
    :autoplay="{
      delay: 4000,
      disableOnInteraction: false,
    }"
    :creative-effect="{
      prev: {
        shadow: false,
        translate: ['-50%', 0, -1],
      },
      next: {
        translate: ['100%', 0, 0],
      },
    }"
  >
    <SwiperSlide v-for="i in 5">
      <div class="relative w-full carousel lg:h-[600px] md:h-60 sm:h-48 h-52">
        <img
          src="https://img.freepik.com/free-photo/painting-mountain-lake-with-mountain-background_188544-9126.jpg"
          class="absolute block w-full h-full object-cover -translate-x-1/2 -translate-y-1/2 top-1/2 left-1/2"
          alt="..."
        />
        <div
          class="flex flex-col pl-[60px] justify-center h-full w-1/2 absolute"
        >
          <h1 class="text-[54px] text-white">
            Modern Interior <br />
            Design Studio
          </h1>
          <div class="h-[50px] mt-[120px] space-x-4 font-medium text-white">
            <button class="px-8 h-full bg-[#027DFC] rounded-[30px]">
              Shop Now
            </button>
            <button class="border-2 border-white px-8 h-full rounded-[30px]">
              Explore
            </button>
          </div>
        </div>
      </div>
    </SwiperSlide>
  </Swiper>
</template>

<script setup></script>

<style lang="scss" scoped></style>
