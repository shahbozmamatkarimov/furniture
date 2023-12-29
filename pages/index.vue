<template>
  <div>
    <section>
      <Slider />
    </section>

    <section class="my-20">
      <h1 class="text-[40px] font-bold">The latest ones</h1>
      <div class="flex items-center justify-between text-lg font-bold">
        <p class="mt-2 text-black/50">
          With over 1 hundred+ furnitures for sale in available on the
          homefinder
        </p>
        <button
          class="h-[40px] bg-[#027DFC] px-8 text-white flex items-center gap-3 rounded-full"
        >
          Show more <img src="@/assets/svg/show_more.svg" alt="" />
        </button>
      </div>

      <div class="flex items-center gap-5 mt-6 overflow-y-auto">
        <div
          v-for="i in 10"
          class="bg-[#F8F8F8] min-w-[300px] h-[393px] p-[10px] rounded-2xl"
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
      <h1 class="text-[40px] font-bold mb-[60px]">New Listed Furnitures</h1>
      <div class="flex items-center gap-8">
        <img src="@/assets/images/furnitures.png" alt="" />
        <div class="max-w-[500px]">
          <h1 class="text-[40px] leading-[40px] font-medium">
            We help you make Modern Interior Design
          </h1>
          <p class="text-[#6A6A6A] text-lg leading-6 mt-7">
            Donec mattis porta eros, aliquet finibus risus interdum at. Nulla
            vivethe as it was for us to know what was to be done. the this is a
            long post for the text.`This small text has to be place here, since
            this is a place holder. You can also chane it.
          </p>
          <ul class="grid grid-cols-2 gap-6 mt-8 text-[#6A6A6A] text-lg">
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
      <h1 class="text-[40px] font-bold w-[380px] leading-[50px]">
        Find Future Space At Budget
      </h1>

      <div class="flex items-center justify-between">
        <div class="flex items-center gap-20 my-9">
          <button
            class="flex items-center justify-center gap-1 font-bold px-5 bg-black rounded-full text-white h-[50px]"
          >
            <img src="@/assets/svg/all.svg" alt="" />
            All
          </button>
          <div class="flex items-center gap-5">
            <button
              class="flex items-center justify-center bg-white gap-1 font-bold px-5 rounded-full h-[50px]"
            >
              Armchairs
            </button>
            <button
              class="flex items-center justify-center bg-white gap-1 font-bold px-5 rounded-full h-[50px]"
            >
              Closets
            </button>
            <button
              class="flex items-center justify-center bg-white gap-1 font-bold px-5 rounded-full h-[50px]"
            >
              Tables
            </button>
          </div>
        </div>
        <button
          class="h-[40px] bg-[#027DFC] px-8 text-white flex items-center gap-3 rounded-full"
        >
          Show more <img src="@/assets/svg/show_more.svg" alt="" />
        </button>
      </div>
      <div class="flex items-center gap-5 overflow-y-auto">
        <div
          v-for="i in 10"
          class="bg-[#F8F8F8] min-w-[300px] h-[393px] p-[10px] rounded-2xl"
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
      <h1 class="text-[#0056AC] font-bold text-lg">JOIN WITH US</h1>
      <p class="text-[32px] font-bold mt-3">Do You Want To Be An Agent?</p>
      <div class="flex items-center justify-between mt-9">
        <p></p>
        <button
          class="h-[40px] bg-[#027DFC] px-8 text-white flex items-center gap-3 rounded-full"
        >
          Show more <img src="@/assets/svg/show_more.svg" alt="" />
        </button>
      </div>
      <div class="flex justify-between mt-3">
        <div>
          <img src="@/assets/images/user1.png" alt="" />
          <div>
            <div class="flex items-center gap-4">
              <img src="@/assets/svg/user_icon.svg" alt="" />
              <h1 class="font-medium text-[32px]">Michael Boy</h1>
            </div>
            <p class="text-black/50 font-medium ml-[63px]">Realstate agent</p>
          </div>
        </div>
        <div class="mt-10">
          <img src="@/assets/images/user2.png" alt="" />
          <div>
            <div class="flex items-center gap-4">
              <img src="@/assets/svg/user_icon.svg" alt="" />
              <h1 class="font-medium text-[32px]">Sophie Rose</h1>
            </div>
            <p class="text-black/50 font-medium ml-[63px]">Realstate agent</p>
          </div>
        </div>
        <div class="mt-20">
          <img src="@/assets/images/user3.png" alt="" />
          <div>
            <div class="flex items-center gap-4">
              <img src="@/assets/svg/user_icon.svg" alt="" />
              <h1 class="font-medium text-[32px]">James watt</h1>
            </div>
            <p class="text-black/50 font-medium ml-[63px]">Realstate agent</p>
          </div>
        </div>
      </div>
    </section>

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
        <p class="mt-3 text-black/40 w-[240px]">1485 Par Drive, Burbank Street , California, CA</p>
        <div class="flex items-center gap-2 mt-6">
          <img src="@/assets/svg/phone.svg" alt="">
          <img src="@/assets/svg/telegram.svg" alt="">
          <img src="@/assets/svg/instagram.svg" alt="">
          <img src="@/assets/svg/youtube.svg" alt="">
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
const images = [
  "https://img.freepik.com/free-photo/painting-mountain-lake-with-mountain-background_188544-9126.jpg",
  "https://us.123rf.com/450wm/hannaklkv/hannaklkv2305/hannaklkv230501239/205670279-vue-panoramique-sur-les-montagnes-enneig%C3%A9es-et-le-lac-bleu-clair.jpg?ver=6",
  "https://img.freepik.com/premium-photo/beautiful-lake-among-mountains-against-backdrop-sunset-dawn_465502-5023.jpg",
];
</script>
