<template>
  <div>
    <section>
      <!-- <Slider /> -->
      <div class="grid lg:grid-cols-4 md:grid-cols-3 sm:grid-cols-2 grid-cols-1 xl:gap-16 gap-5 -mx-[10px] mt-10">
        <div
          v-for="i in 10"
          class="bg-[#F8F8F8] max-w-[300px] h-[393px] p-[10px] rounded-2xl mx-auto"
        >
          <img
            class="rounded-[12px] w-[279px] h-[282px] object-cover"
            src="@/assets/images/furniture.png"
            alt=""
          />
          <ul class="flex items-center gap-8 my-[10px] h-4 text-sm font-medium">
            <li class="flex items-center gap-1">
              <img src="@/assets/svg/heart.svg" alt="" />
              <p>16</p>
            </li>
            <li class="flex items-center gap-1">
              <img src="@/assets/svg/watched.svg" alt="" />
              <p>16</p>
            </li>
            <li class="flex items-center gap-1">
              <img src="@/assets/svg/comment.svg" alt="" />
              <p>16</p>
            </li>
          </ul>
          <h1 class="text-lg font-bold leading-4 mb-[10px]">
            Richmond Appartment
          </h1>
          <ul class="flex items-center justify-between">
            <li class="text-lg font-bold">$985,000</li>
            <li class="flex items-center gap-3">
              <img src="@/assets/svg/heart_white.svg" alt="" />
              <img src="@/assets/svg/cart.svg" alt="" />
            </li>
          </ul>
        </div>
      </div>
    </section>
  </div>
</template>
