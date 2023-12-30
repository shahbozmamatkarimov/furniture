<template>
  <nav class="fixed whitespace-nowrap bg-white w-full z-50 h-[90px]">
    <div
      class="right-0 left-0 flex justify-between items-center h-[90px] font-medium py-3 container md:px-10 px-5 mx-auto"
    >
      <router-link to="/"><img src="/logo.svg" /></router-link>
      <ul class="xl:flex hidden gap-16 text-2xl">
        <li>
          <router-link to="/"
            >Home
            <p
              class="hidden bg-[#027DFC] mt-[8px] -mb-[8px] w-[70%] h-[3px]"
            ></p
          ></router-link>
        </li>
        <li>
          <router-link to="/services">
            Services
            <p
              class="hidden bg-[#027DFC] mt-[8px] -mb-[8px] w-[70%] h-[3px]"
            ></p>
          </router-link>
        </li>
        <li>
          <router-link to="/about_us">
            About us
            <p
              class="hidden bg-[#027DFC] mt-[8px] -mb-[8px] w-[70%] h-[3px]"
            ></p>
          </router-link>
        </li>
        <li>
          <router-link to="/contact_us">
            Contact us
            <p
              class="hidden bg-[#027DFC] mt-[8px] -mb-[8px] w-[70%] h-[3px]"
            ></p>
          </router-link>
        </li>
      </ul>
      <ul class="flex gap-3 text-[11px]">
        <li @click="store.navbar = true" v-show="!store.navbar" class="xl:hidden block px-5 py-2 bg-[#E0EBED] rounded-[10px]">
          <img src="@/assets/svg/menu.svg" />
          <p class="text-center">Menu</p>
        </li>
        <li @click="store.navbar = false" v-show="store.navbar" class="xl:hidden block  px-5 py-2 bg-[#E0EBED] rounded-[10px]">
          <img src="@/assets/svg/close_menu.svg" />
          <p class="text-center">Menu</p>
        </li>
        <li class="sm:block hidden px-5 py-2 bg-[#E0EBED] rounded-[10px]">
          <img src="@/assets/navbar/lang.svg" />
          <p class="text-center">English</p>
        </li>
        <li class="sm:block hidden px-5 py-2 bg-[#E0EBED] rounded-[10px]">
          <img src="@/assets/navbar/heart.svg" />
          <p class="text-center">Likes</p>
        </li>
        <li class="sm:block hidden px-5 py-2 bg-[#E0EBED] rounded-[10px]">
          <img src="@/assets/navbar/cart.svg" />
          <p class="text-center">Cart</p>
        </li>
      </ul>
    </div>

    <ul v-if="store.navbar" class="xl:hidden !pb-40 flex flex-col container md:py-16 sm:py-10 py-5 md:px-10 px-5 mx-auto overflow-hidden overflow-y-auto bg-white h-[calc(100vh_-_80px)] text-[40px] leading-normal gap-16 text-2xl">
      <li data-aos="fade-left">
        <router-link to="/"
          >Home
          <p class="hidden bg-[#027DFC] mt-[8px] -mb-[8px] w-[70%] h-[3px]"></p
        ></router-link>
      </li>
      <li data-aos="fade-up">
        <router-link to="/services">
          Services
          <p class="hidden bg-[#027DFC] mt-[8px] -mb-[8px] w-[70%] h-[3px]"></p>
        </router-link>
      </li>
      <li data-aos="fade-down">
        <router-link to="/about_us">
          About us
          <p class="hidden bg-[#027DFC] mt-[8px] -mb-[8px] w-[70%] h-[3px]"></p>
        </router-link>
      </li>
      <li data-aos="fade-right" data-duration="500">
        <router-link to="/contact_us">
          Contact us
          <p class="hidden bg-[#027DFC] mt-[8px] -mb-[8px] w-[70%] h-[3px]"></p>
        </router-link>
      </li>
      <li class="sm:hidden block">
        <ul class="flex gap-3 text-[11px]">
          <li class="px-5 py-2 bg-[#E0EBED] rounded-[10px]">
            <img src="@/assets/navbar/lang.svg" />
            <p class="text-center">English</p>
          </li>
          <li class="px-5 py-2 bg-[#E0EBED] rounded-[10px]">
            <img src="@/assets/navbar/heart.svg" />
            <p class="text-center">Likes</p>
          </li>
          <li class="px-5 py-2 bg-[#E0EBED] rounded-[10px]">
            <img src="@/assets/navbar/cart.svg" />
            <p class="text-center">Cart</p>
          </li>
        </ul>
      </li>
    </ul>
  </nav>
</template>

<script setup>
const store=reactive({
  navbar: false,
})

const router = useRouter();

watch(() => router.currentRoute.value, () => {
  store.navbar = false;
})
</script>

<style lang="scss">
ul li {
  cursor: pointer;
}

.router-link-exact-active {
  p {
    display: block;
  }
}
</style>
