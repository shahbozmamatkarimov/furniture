<template>
  <div>
    <section>
      <Slider />
    </section>

    <section class="my-20">
      <h1 data-aos="fade-up" class="md:text-[40px] text-[32px] font-bold">
        The latest ones
      </h1>
      <div
        class="md:flex gap-5 md:space-y-0 space-y-2 items-center justify-between text-lg font-bold"
      >
        <p data-aos="fade-right" class="mt-2 md:text-[16px] text-sm text-black/50">
          With over 1 hundred+ furnitures for sale in available on the
          homefinder
        </p>
        <button data-aos="fade-left"
          class="h-[40px] bg-[#027DFC] whitespace-nowrap px-8 text-white flex items-center gap-3 rounded-full"
        >
          Show more <img src="@/assets/svg/show_more.svg" alt="" />
        </button>
      </div>

      <div class="flex items-center gap-5 mt-6 overflow-y-auto">
        <div data-aos="fade-up"
          v-for="i in 10"
          @click="$router.push('/products/' + i)"
          class="cursor-pointer bg-[#F8F8F8] min-w-[300px] h-[393px] p-[10px] rounded-2xl"
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

    <section>
      <h1 data-aos="fade-up" class="md:text-[40px] text-[32px] font-bold mb-[60px]">
        New Listed Furnitures
      </h1>
      <div class="md:flex items-center gap-8">
        <img data-aos="fade-right" class="md:w-[50%]" src="@/assets/images/furnitures.png" alt="" />
        <div data-aos="fade-left" class="max-w-[500px]">
          <h1 class="lg:text-[40px] text-[28px] leading-[40px] font-medium">
            We help you make Modern Interior Design
          </h1>
          <p class="text-[#6A6A6A] lg:text-lg leading-6 lg:mt-7 mt-4">
            Donec mattis porta eros, aliquet finibus risus interdum at. Nulla
            vivethe as it was for us to know what was to be done. the this is a
            long post for the text.`This small text has to be place here, since
            this is a place holder. You can also chane it.
          </p>
          <ul
            class="grid grid-cols-2 lg:gap-6 gap-4 lg:mt-8 mt-4 text-[#6A6A6A] lg:text-lg"
          >
            <li class="flex items-center gap-3">
              <img class="w-2" src="@/assets/svg/list_icon.svg" alt="" />Donec
              mattis porta eros,let aliquet finibus ri
            </li>
            <li class="flex items-center gap-3">
              <img class="w-2" src="@/assets/svg/list_icon.svg" alt="" />Donec
              mattis porta eros,let aliquet finibus ri
            </li>
            <li class="flex items-center gap-3">
              <img class="w-2" src="@/assets/svg/list_icon.svg" alt="" />Donec
              mattis porta eros,let aliquet finibus ri
            </li>
            <li class="flex items-center gap-3">
              <img class="w-2" src="@/assets/svg/list_icon.svg" alt="" />Donec
              mattis porta eros,let aliquet finibus ri
            </li>
          </ul>
        </div>
      </div>
    </section>

    <section class="bg-[#F5EEE8] py-10 -mx-[50vw] px-[50vw] my-20">
      <h1 data-aos="fade-up"
        class="md:text-[40px] sm:text-[32px] text-[28px] font-bold sm:w-[380px] leading-[50px]"
      >
        Find Future Space At Budget
      </h1>

      <div class="md:flex items-center justify-between whitespace-nowrap">
        <div data-aos="fade-right"
          class="flex items-center overflow-hidden overflow-x-auto md:gap-20 gap-10 my-9"
        >
          <button
            class="flex items-center justify-center gap-1 font-bold px-5 bg-black rounded-full text-white md:h-[50px] h-[40px]"
          >
            <img src="@/assets/svg/all.svg" alt="" />
            All
          </button>
          <div class="flex items-center gap-5">
            <button
              class="flex items-center justify-center bg-white gap-1 font-bold px-5 rounded-full md:h-[50px] h-[40px]"
            >
              Armchairs
            </button>
            <button
              class="flex items-center justify-center bg-white gap-1 font-bold px-5 rounded-full md:h-[50px] h-[40px]"
            >
              Closets
            </button>
            <button
              class="flex items-center justify-center bg-white gap-1 font-bold px-5 rounded-full md:h-[50px] h-[40px]"
            >
              Tables
            </button>
          </div>
        </div>
        <button data-aos="fade-left"
          class="h-[40px] md:mb-0 mb-2 bg-[#027DFC] px-8 text-white flex items-center gap-3 rounded-full"
        >
          Show more <img src="@/assets/svg/show_more.svg" alt="" />
        </button>
      </div>
      <div class="flex items-center gap-5 overflow-y-auto">
        <div data-aos="fade-up"
          v-for="i in 10"
          @click="$router.push('/products/' + i)"
          class="cursor-pointer bg-[#F8F8F8] min-w-[300px] h-[393px] p-[10px] rounded-2xl"
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

    <section>
      <h1 data-aos="fade-up" class="text-[#0056AC] font-bold text-lg">JOIN WITH US</h1>
      <p data-aos="fade-right" class="text-[32px] font-bold mt-3">Do You Want To Be An Agent?</p>
      <div class="flex items-center justify-between mt-9">
        <p></p>
        <button data-aos="fade-left"
          class="h-[40px] bg-[#027DFC] px-8 text-white flex items-center gap-3 rounded-full"
        >
          Show more <img src="@/assets/svg/show_more.svg" alt="" />
        </button>
      </div>
      <div
        class="flex justify-between mt-3 md:text-[32px] sm:text-[16px] text-xs"
      >
        <div data-aos="fade-right">
          <img src="@/assets/images/user1.png" alt="" />
          <div>
            <div class="flex items-center gap-4">
              <img
                class="md:block hidden"
                src="@/assets/svg/user_icon.svg"
                alt=""
              />
              <h1 class="font-medium md:leading-7">Michael Boy</h1>
            </div>
            <p class="text-black/50 font-medium md:leading-7 md:ml-[63px]">
              Realstate agent
            </p>
          </div>
        </div>
        <div data-aos="fade-up" class="mt-10">
          <img src="@/assets/images/user2.png" alt="" />
          <div>
            <div class="flex items-center gap-4">
              <img
                class="md:block hidden"
                src="@/assets/svg/user_icon.svg"
                alt=""
              />
              <h1 class="font-medium md:leading-7">Sophie Rose</h1>
            </div>
            <p class="text-black/50 font-medium md:leading-7 md:ml-[63px]">
              Realstate agent
            </p>
          </div>
        </div>
        <div data-aos="fade-left" class="mt-20">
          <img src="@/assets/images/user3.png" alt="" />
          <div>
            <div class="flex items-center gap-4">
              <img
                class="md:block hidden"
                src="@/assets/svg/user_icon.svg"
                alt=""
              />
              <h1 class="font-medium md:leading-7">James watt</h1>
            </div>
            <p class="text-black/50 font-medium md:leading-7 md:ml-[63px]">
              Realstate agent
            </p>
          </div>
        </div>
      </div>
    </section>

    <Footer />
  </div>
</template>

<script>
const images = [
  "https://img.freepik.com/free-photo/painting-mountain-lake-with-mountain-background_188544-9126.jpg",
  "https://us.123rf.com/450wm/hannaklkv/hannaklkv2305/hannaklkv230501239/205670279-vue-panoramique-sur-les-montagnes-enneig%C3%A9es-et-le-lac-bleu-clair.jpg?ver=6",
  "https://img.freepik.com/premium-photo/beautiful-lake-among-mountains-against-backdrop-sunset-dawn_465502-5023.jpg",
];
</script>
