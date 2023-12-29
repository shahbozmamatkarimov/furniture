<template>
  <nav class="fixed bg-white w-full z-50 h-[90px]">
    <div
      class="right-0 left-0 flex justify-between items-center h-[90px] font-medium py-3 container px-10 mx-auto"
    >
      <router-link to="/"><img src="/logo.svg" /></router-link>
      <ul class="flex gap-16 text-2xl">
        <li>
          <router-link to="/"
            >Home
            <p class="hidden bg-[#027DFC] mt-[8px] -mb-[8px] w-[70%] h-[3px]"></p
          ></router-link>
        </li>
        <li>
          <router-link to="/services">
            Services
            <p class="hidden bg-[#027DFC] mt-[8px] -mb-[8px] w-[70%] h-[3px]"></p>
          </router-link>
        </li>
        <li>
          <router-link to="/about_us">
            About us
            <p class="hidden bg-[#027DFC] mt-[8px] -mb-[8px] w-[70%] h-[3px]"></p>
          </router-link>
        </li>
        <li>
          <router-link to="/contact_us">
            Contact us
            <p class="hidden bg-[#027DFC] mt-[8px] -mb-[8px] w-[70%] h-[3px]"></p>
          </router-link>
        </li>
      </ul>
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
    </div>
  </nav>
</template>

<script></script>

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
